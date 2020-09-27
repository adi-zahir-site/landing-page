<template>
  <div id="contact" class="jumbotron">
    <img class="studio-img" alt="סטודיו" src="../../assets/studio.jpg" />

    <div class="content">
      <div class="row">
        <div class="col">
          <div class="row d-flex justify-content-center">
            <div class="col-md-11">
              <h1>צרו קשר</h1>
              <hr />
            </div>
          </div>
          <div id="contact-details" class="row d-flex justify-content-center">
            <div class="col-md-11">
              <div>
                <i class="fa fa-phone ml-2"></i>
                טלפון: <a href="tel:0522981168">052-2981168</a>
              </div>
              <div>
                <i class="fa fa-envelope ml-2"></i>
                אימייל:
                <a href="mailto:adizahir4@gmail.com">adizahir4@gmail.com</a>
              </div>
              <div>
                <i class="fa fa-map-marker ml-2"></i>
                כתובת: בן גוריון 199, רמת גן
              </div>
            </div>
          </div>
          <div class="row mt-12 d-flex justify-content-center">
            <div class="col-md-11">
              <h3>עקבו אחרי:</h3>
              <a
                href="https://www.facebook.com/Adi-Zahir-Personal-trainer-104459667751202/"
                target="_blank"
                ><button
                  type="button"
                  class="btn btn-social-icon btn-outline-facebook mt-12"
                >
                  <i class="fa fa-facebook"></i></button
              ></a>
              <a href="https://www.instagram.com/adi_zahir/" target="_blank"
                ><button
                  type="button"
                  class="btn btn-social-icon btn-outline-instagram mt-12"
                >
                  <i class="fa fa-instagram"></i></button
              ></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style scoped>
#contact {
  font-size: 20px;
  line-height: 2;
  direction: rtl;
  text-align: justify;
  position: relative;
  overflow: hidden;
  margin-bottom: 0;
  background-color: #FFC400;
}

.content {
  z-index: 2;
}

#contact-details .fa {
  width: 20px;
  text-align: right;
}

.btn-social-icon {
  color: #343a40;
  font-size: 40px;
  width: 80px;
  height: 80px;
  margin-left: 20px;
  border: 3px solid #343a40;
}

.btn-social-icon a {
  color: #343a40;
}

.btn-social-icon:hover a {
  color: whitesmoke;
}

.btn-social-icon:hover {
  color: whitesmoke;
  border-color: whitesmoke;
}

.studio-img {
  position: absolute;
  left: 0;
  top: 0;
  width: 140%;
  opacity: 0.15;
}
</style>
