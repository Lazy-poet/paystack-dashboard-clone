<template>
  <div class="content-container container">
 <div class="row top-row">
     <div class="col col-lg-8 col-md-12 top-col">
        <h3>Welcome to Paystack</h3>
        <h4>Your business is in test mode</h4>
     </div>
 </div>
    <div class="cards">
      <div class="card">
        <div class="icon">
          <svg
            width="25"
            height="25"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M4.5 15.5s1-1 4-1 5 2 8 2 4-1 4-1v-12s-1 1-4 1-5-2-8-2-4 1-4 1v12zM4.5 22.5v-7"
              stroke="#3bb75e"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            ></path>
          </svg>
        </div>
        <h5 class="desc">Submit compliance details to accept live payments</h5>
        <button class="btn btn-success card-button">Activate business</button>
      </div>
      <div class="card">
        <div class="icon">
          <svg
            width="25"
            height="25"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M18.5 21.5a3 3 0 100-6 3 3 0 000 6zM6.5 9.5a3 3 0 100-6 3 3 0 000 6zM13.5 6.5h3a2 2 0 012 2v7M6.5 9.5v12"
              stroke="#3bb75e"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            ></path>
          </svg>
        </div>
        <h5 class="desc">Learn what you can do with the Paystack Dashboard</h5>
        <button class="btn btn-light btn-outline-secondary card-button">
          Take a tour
        </button>
      </div>
      <div class="card">
        <div class="icon">
          <svg
            width="25"
            height="25"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M12.5 22.5c5.523 0 10-4.477 10-10s-4.477-10-10-10-10 4.477-10 10 4.477 10 10 10z"
              stroke="#3bb75e"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            ></path>
            <path
              d="M12.5 16.5a4 4 0 100-8 4 4 0 000 8zM5.43 5.43l4.24 4.24M15.33 15.33l4.24 4.24M15.33 9.67l4.24-4.24M15.33 9.67l3.53-3.53M5.43 19.57l4.24-4.24"
              stroke="#3bb75e"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            ></path>
          </svg>
        </div>
        <h5 class="desc">Find answers to questions you might have or get in touch</h5>
        <button class="btn btn-light btn-outline-secondary card-button">
          Go to Support
        </button>
      </div>
    </div>
    <div class="bottom-row row">
      <div class="col-lg-10 col-md-12">
       <div class="wrapper">
          <div class="row">
            <div class=" m-col-sm">
             <div class="documentation">
                <h4 class="doc-header">API Documentation</h4>
                <p class="doc-body">
                  Our documentation contains the Libraries, APIs, and SDKs you need
                  to integrate Paystack in your website or app.
                </p>
                <button class="btn btn-light btn-outline-secondary">
                  Go to Docs
                </button>
             </div>
            </div>
            <div class="m-col-sm">
              <div class="test-keys ">
              <h4 class="test-header">Your Test Keys</h4>
              <p class="test-body">
                Also available in <a> Settings > API Keys & Webhooks</a>
              </p>
              <div class="input-group mb-3">
                <div class="input-group-prepend">
                  <span class="input-group-text">Test Secret</span>
                </div>
                <input
                  type="text"
                  class="form-control"
                  value="My key"
                  readonly
                />
                <div class="input-group-append">
                  <span class="input-group-text">Copy</span>
                </div>
              </div>
              <div class="input-group mb-3">
                <div class="input-group-prepend">
                  <span class="input-group-text">Test Public</span>
                </div>
                <input
                  type="text"
                  class="form-control"
                  value="My key"
                  readonly
                />
                <div class="input-group-append">
                  <span class="input-group-text">Copy</span>
                </div>
              </div>
            </div>
          
            </div>
            </div>
       </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "GetStarted",
};
</script>
<style scoped>
.content-container {
  box-sizing: border-box;
  height: 100%;
  padding-top: 20px;
  display: flex;
  flex-direction: column;
  
  align-items: center;
  min-width: 960px;

  flex: 1;
}
.top-row{
  display: block;
  width: 100%;
  margin-bottom: 20px;
  padding: 10px;
}
.top-col{
  display: block;
 margin: auto;
 padding-top: 20px;
  text-align: center;
}
h3 {
  font-size: 21px;
  font-weight: 500;
  margin-bottom: 8px;
color: #57584e;
  letter-spacing: -0.1px;
}

h4 {
  color: #777;
  font-size: 16px;
  line-height: 1.5;
  font-weight: 400;
  margin: 0;
}
.cards {
  display: grid;
  place-items: center;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 20px;


  /* flex-basis: 0;
  flex-grow: 1;
  align-items: center;
  justify-content: center; */
}
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  width: 300px;
  height: 300px;
  padding: 50px;
  border: 1px solid #f2f2f2;
  border-radius: 3px;
  text-align: center;
  background: #fff;
}

.icon {
  height: 60px;
  width: 60px;
  background: #f1fbf4;
  color: #3bb75e;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.card h5 {
  display: inline-block;
  width: 100%;
  color: #727366;
  font-size: 13.5px;
  line-height: 1.5;
  font-weight: 400;
  margin: 20px 0;
  padding: 0px !important;
  
}

.btn {
  font-size: 13px;
  margin-top: 10px;
  height: 36px;
  padding: 0 16px;
  border-radius: 5px;
  outline: 0;
  border: 1px solid rgba(0, 0, 0, 0.2);
  display: inline-flex;
  align-items: center;
  justify-content: center;

}
.btn-success{
  background-color: #3bb75e;
  border-color: #3bb75e;
 
}
.bottom-row > div{
  margin: 60px auto 0
}
.wrapper{
  padding: 30px;
  margin-top: 20px;
  border-color: #edf1f2;
  border-top: 1px solid #dee5e7 ;
}
.m-col-sm{
  width: 50%;
  padding: 0 15px;
  position: relative


}
.test-keys, .documentation {
  padding: 0 15px;
}
.doc-header, .test-header{
  font-size: 16px;
  font-weight: 500;
  margin-bottom: 10px;
  line-height: 1.1;
  color: #57584e;
  font-family: inherit;
}
.doc-body{
  font-size: 15px;
  margin: 0 0 10px;
  color: #727366
}

.test-body{
  color: #a4a59a;
  margin: 0 0 10px;
  font-size: 14px
}
.test-body a {
  color: #3676c8;
  text-decoration: none;
  cursor: pointer
}
.input-group{
  margin-bottom: 10px;
}
.input-group-text{
  font-size: 14px;
  line-height: 1;
  padding: 6px 12px;
  font-weight: 400;
  color: #555;
  border: 1px solid transparent;
  border-color: #dee5e7;
  background: #edf1f2;
  vertical-align: middle;
  white-space: nowrap;

}
.form-control{
  padding: 6px 12px;
  height: 34px;
  
  border: 1px solid internal-light-dark(rgb(118, 118, 118), rgb(133, 133, 133));
  background:#fff;
    text-rendering: auto;
    color:#989898;
    letter-spacing: normal;
    word-spacing: normal;
    text-transform: none;
    text-indent: 0px;
    text-shadow: none;
    text-align: start;
    appearance: auto;

}

@media (min-width: 1024px){
  .top-row{
    padding: 20px
    }
}
</style>