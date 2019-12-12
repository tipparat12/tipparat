# tipparat
onst request = require('request')

request({
  method: 'POST',
  uri: 'https://notify-api.line.me/api/notify',
  header: {
    'Content-Type': 'application/x-www-form-urlencoded',
  },
  auth: {
    bearer: 's9LxGD6EVVeK7v0vqp8KUmMMeAq3dRqjmlFKFe9azN8', 
  },
  form: {
    message: 'ทดสอบ', 
  },
}, (err, httpResponse, body) => {
  if (err) {
    console.log(err)
  } else {
    console.log(body)
  }
})
