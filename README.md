# fetch api
####  GET
      fetch('https://jsonplaceholder.typicode.com/todos')
            .then((res) => {
                res.json().then((result) => {
                    console.log(result)
                })
            })
            .catch(err=> console.error(err));

####  POST

