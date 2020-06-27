# graphql-union-types

---

- http://localhost:4000/

```js
query {
  agenda {
    __typename
    ...StudyGroupFields
    ...WorkoutFields
  }
}

fragment StudyGroupFields on StudyGroup {
  name
  subject
  students
}

fragment WorkoutFields on Workout {
  name
  reps
}

```
