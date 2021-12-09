<template>
  <section>
    <section class="jumbotron jumbotron--center" style="background-image: linear-gradient(rgba(0,0,0,.5), rgba(0,0,0,.5)), url('img/IMG_4130-scaled.jpg');">
      <h1 class="jumbotron__heading">Contact Us</h1>
    </section>
    <section class="section">
      <div class="heading-group">
        <h3 class="heading heading--fancy">request a call back</h3>
        <h1 class="heading section__heading">contact us today</h1>
      </div>
      <div class="row m-0 justify-content-between">
        <div class="col-md-8 p-0">
          <form class="form" @submit.prevent="sendMail()">
            <h2 class="form__heading">message</h2>
            <div class="row m-0">
              <div class="col-md-6">
                <input type="text" class="form__input" placeholder="Full Name" v-model="contact.name" />
              </div>
              <div class="col-md-6">
                <input type="email" class="form__input" placeholder="Email Address" v-model="contact.mail" />
              </div>
              <div class="col-md-6">
                <input type="tel" class="form__input" placeholder="Phone Number" v-model="contact.phone" />
              </div>
              <div class="col-md-6">
                <input type="text" class="form__input" placeholder="Company Name" v-model="contact.company" />
              </div>
              <div class="col-md-12">
                <textarea class="form__input form__input--big" placeholder="Message"  v-model="contact.message">
                </textarea>
              </div>
              <div class="col-md-12">
                <button type="submit" class="btn btn--black">submit</button>
              </div>
            </div>
          </form>
        </div>
        <div class="col-md-3 p-0">
          <h2 class="form__heading">our contact</h2>
          <div class="d-flex align-items-middle">
            <i class="fa fa-phone"></i>&nbsp;&nbsp;&nbsp;&nbsp;
            <span>440-349-4020</span>
          </div>
          <div class="d-flex align-items-middle mt-5">
            <i class="fa fa-envelope"></i>&nbsp;&nbsp;&nbsp;&nbsp;
            <span>sales@pressurecomponent.com</span>
          </div>
        </div>
      </div>
    </section>
    {{ contact }}
  </section>
</template>

<script>
export default {
  name: 'ContactUsPage',
  data() {
    return {
      contact: {}
    }
  },
  methods: {
    sendMail() {
      let data = this.contact/*
      const response = fetch('//8s26c6wvrb.execute-api.us-east-2.amazonaws.com/prod/mailsend', {
        method: 'POST',
        host: 443,
        headers: {'Content-Type': 'application/json'},
        body: JSON.stringify(data)
      });
      return response;*/

      // Example POST method implementation:
async function postData(url = '', data = {}) {
  // Default options are marked with *
  const response = await fetch(url, {
    method: 'POST', // *GET, POST, PUT, DELETE, etc.
    mode: 'no-cors', // no-cors, *cors, same-origin
    cache: 'no-cache', // *default, no-cache, reload, force-cache, only-if-cached
    //credentials: 'same-origin', // include, *same-origin, omit
    headers: {
      'Content-Type': 'application/json'
      // 'Content-Type': 'application/x-www-form-urlencoded',
    },
    redirect: 'follow', // manual, *follow, error
    referrerPolicy: 'no-referrer', // no-referrer, *no-referrer-when-downgrade, origin, origin-when-cross-origin, same-origin, strict-origin, strict-origin-when-cross-origin, unsafe-url
    body: JSON.stringify(data) // body data type must match "Content-Type" header
  });
  return response.json(); // parses JSON response into native JavaScript objects
}

postData('//8s26c6wvrb.execute-api.us-east-2.amazonaws.com/prod/mailsend:443', this.contact)
  .then(data => {
    console.log(data); // JSON data parsed by `data.json()` call
  });

    }
  }
}
</script>

<style>

</style>