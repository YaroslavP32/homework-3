My answers:
1.  db.sample.find({'scores': {$elemMatch: {score: {$gt: 87, $lt: 93}}}})

2.  db.test.aggregate([{$unwind: "$scores"}, {$match: {'scores.type': "exam", 'scores.score': {$gt: 90}}}])

3.  db.test.update({"name": "Dusti Lemmond"}, {$set: {"accepted": "true"}}, {multi: true})
               
               
               
               
               
               
               
               
               
               
               
              