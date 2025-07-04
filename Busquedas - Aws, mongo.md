**AWS**

| filter (_@message_ like 'hdToQCSf9GBvGMXmz' or _@message_ like '17413174') and _@message_ not like '(resolver)' and _@message_ not like 'About to update delivery' and _@message_ not like 'Check delivery'

  

fields _@timestamp_, _@message_, _@logStream_, _@log_

| filter level = 'error'

| stats count(*) as count group by message

| sort count desc

| limit 100

  

**Queries Mongo**

Diccionario de los eventos que se guardan en la colletions log (MongoDB)

  

db.getCollection("api.logs").find({websiteId:"5Qqgdwu7EePBkkSX5", date:{$gte:ISODate('2024-02-13'), $lt:ISODate('2024-02-14')}, method:{ $in: [ "deliverectMenu", "setListing"]}})

  

db.getCollection("orders"). find({code: "17259245"})

db.getCollection("order_items"). find ({orderId: "sDDHSdTSjmTDzhhgF"})

  

{websiteId:"zk3q6Kf4f9oH6gr6g", method: { $nin: ["orders", "acceptOrder", "listing", "pendingOrders", "outOfStockItems", "me", "rejectOrder", "stores"] }, date:{$gte:ISODate('2024-02-12'), $lt:ISODate('2024-02-13')} }

  

db.products. find({_id: "4uRaZwa9550yWHnw8"})

db.getCollection("products .modifiers").find({_id: {$in: ["M4jD8ZJLb3MkpSxzs", "EGpRWPjbnRe2SanAC”]}}). 

db.getCollection("products .modifier_options").find({_id: {$in: ["×3XQCjHy82Mv7sdkh", "Ltou56JRYTZjKPRGc" 1}})

db.users.find({_id: "NygMu2k4428mesu8D"})

  

db.getCollection(“main.orders”).find ({meta.specialCode : E10223 })

db.getCollection(“main.delivereries”).find ({externalId: el que saque de orders})

  

db.getCollection(“main.delivereries”).find {websiteId:'k6n4fJLLrfMFmWQF8', _id: {$in:['7BnCuFRSKKkJ3Zdrc', 'egYMST6zY2bfPeeAH', 'TkznG2hRDwkWBgMWu', 'Zqvu7dgbKSTEEGtba']}}

  

method: { $ne: ["orders", "acceptOrder"]}

es que el $ne es para valores exactos

en este caso tienes que usar un $nin

o algo así

eso funciona para arreglos

Acá una de ejemplo con Logs.

{createdAt: {$gte: ISODate('2024-02-01')}, method: { $nin: ["orders", "acceptOrder"]}}

db.collection.find({ "responseText": { $regex: /store not found/ } })

  

{websiteId: 'DL22WcZWu48QEBByA', responseText: {$regex: 'NKKfxssTdw5DGWKXS'}}

  

.**sort({**date**:**-1**}) para que muestre la fecha de hoy**

  

{$text: {$search: 'id_aca'}} para buscar el pago asociado

