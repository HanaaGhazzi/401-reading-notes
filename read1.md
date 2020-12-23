# Review, Research, and Discussion

## Array.map() 
 
 _Generally map() method is used to iterate over an array and calling function on every element of array._

### The syntax of the map() method is:

```
arr.map(callback(currentValue), thisArg)
```
Here, ```arr``` is an array.

## Array.reduce()

_The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in single output value._


### The syntax of the reduce() method is : 

```
arr.reduce(callback( accumulator, currentValue, [, index[, array]] )[, initialValue])
```

## superagent: 
 
 _this example from our project_

### .then
```
function coursesHandler(req, res) {
  let URL = `https://www.udemy.com/api-2.0/courses/?category=Photography+%26+Video&page=1&page_size=12&price=price-free`;
  superagent(URL)
    .set('Authorization', `Basic ${Buffer.from(`${process.env.UDEMEM_CLIENT}:${process.env.UDEMEY_SECRET}`).toString('base64')}`)
    .then(result => {
      let courses = result.body.results.map(val => {
        return new Course(val);

      });
      if (req.user) {
        res.render('courses', { LoggedIn: true, courses: courses, user: req.user, pageName: 'Recommended Courses' })
      }
      else {
        res.status(200).render('courses', { LoggedIn: false, courses: courses, pageName: 'Recommended Courses' });
      }
    }).catch((e) => {
      res.status(500).send(e);
    });
}

``` 
### async & await :
```
async function homeHandler(req, res) {
  let pictureOfTheDay = await natgeo.getPhotoOfDay(`DAY`, `CALLBACK`)
    .then((result) => {
      return result.data[0].attributes;
    });

```

## What is a Promise?

**A promise is an object that may produce a single value some time in the future: either a resolved value, or a reason that it’s not resolved (e.g., a network error occurred). A promise may be in one of 3 possible states: fulfilled, rejected, or pending. Promise users can attach callbacks to handle the fulfilled value or the reason for rejection.**

## Are all callback functions considered to be Asynchronous? Why or Why Not?

Simply taking **a callback doesn't make a function asynchronous.** There are many examples of functions that take a function argument but are not asynchronous. For example there's forEach in Array. It iterates over each item and calls the function once per item 

_For a function to be asynchronous it needs to perform an asynchronous operation. It needs to incorporate the argument callback in handling the results of this asynchronous operation. Only this way the function becomes asynchronous._


