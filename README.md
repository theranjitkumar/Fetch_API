#  Fetch API
####  GET
      fetch('https://jsonplaceholder.typicode.com/posts')
            .then((res) => {
                res.json().then((result) => {
                    console.log(result)
                })
            })
            .catch(err=> console.error(err));

####  POST

            var data = {
              title: 'Test Title',
              body: 'Test body ....'
            };

            fetch('https://jsonplaceholder.typicode.com/posts', {
                method: 'POST', // or 'PUT'
                body: JSON.stringify(data), // data can be `string` or {object}!
                headers:{
                  'Content-Type': 'application/json'
                }
              }).then(res => res.json())
              .then(response => console.log('Success:', JSON.stringify(response)))
              .catch(error => console.error('Error:', error));
