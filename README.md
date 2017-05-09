# fetch_promise

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>JS Bin</title>
</head>
<body>
<script>
fetch('https://raw.githubusercontent.com/theranjitkumar/jsonData/master/jsonData.json')
  .then((res)=>{
  res.json().then((result)=>{
    console.log(result)
  })
})  
</script>
</body>
</html>
