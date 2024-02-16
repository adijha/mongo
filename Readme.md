##script to make all email lowercase

db.pointsdataschemas.updateMany(
   {},
   [
     { $set: { email: { $toLower: "$email" } } }
   ]
)
