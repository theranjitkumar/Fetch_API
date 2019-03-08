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

            var data = {
                "userId": 1,
                "id": 1,
                "title": "delectus aut autem",
                "completed": false
              };

            fetch('https://jsonplaceholder.typicode.com/todos', {
                method: 'POST', // or 'PUT'
                body: JSON.stringify(data), // data can be `string` or {object}!
                headers:{
                  'Content-Type': 'application/json'
                }
              }).then(res => res.json())
              .then(response => console.log('Success:', JSON.stringify(response)))
              .catch(error => console.error('Error:', error));
