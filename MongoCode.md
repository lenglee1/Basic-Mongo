#Mongo Snippets
##Querying across collections

```
var x = db.lessons.findOne()
x
db.courses.findOne(x.course_id)

db.courses.findOne(db.lessons.findOne().course_id)
```