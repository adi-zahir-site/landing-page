<template>
  <div class="position-relative">
    <div id="about" class="about jumbotron">
      <div class="row">
        <div class="col-lg-6">
          <div>
            <p class="about-text fade-in">
              נעים להכיר! אני עדי, בת 25, בעלת סטודיו בוטיק לאימוני כוח לקבוצות
              ויחידים ברמת גן.<br />
              שירתתי בצבא בתור קצינת אימון גופני לתקופה משמעותית של שלוש שנים,
              במהלכן, עוד לפני שהשתחררתי, ידעתי בדיוק מה אני הולכת לעשות - לפתוח
              את סטודיו החלומות שלי, סטודיו AZ.<br />
              לאחר שהשתחררתי הכנתי את הקרקע לבניית הסטודיו, וחשבתי כיצד להביא את
              ה״אני מאמין״ שלי כמאמנת לתוך האימונים שלי.<br />
              אני מאמינה שבכל עולם הכושר יש משהו מעבר ללהכנס לכושר; ההחלטה
              להתחיל להתאמן היא תהליך אישי, מסע של למידה שכולו התפתחות והעצמה
              אישית. במהלך האימונים אנחנו משחררים את ה״טייס האוטומטי״ והשגרה
              השוחקת ומתחילים להשתמש ולהרגיש כל איבר ואיבר בגוף. הטכניקה והחיבור
              עם המוח (המחשבה) לגוף הם מעל הכל. המטרה המשותפת שלנו בתהליך היא
              להטמיע הרגלים ספורטיביים שיהפכו להיות חלק משגרת חיינו. יחד, נלמד
              להיות חזקים ובריאים יותר כאשר אנחנו משתמשים ב״מכונה״ המדהימה
              שנקראת הגוף שלנו.<br />

              עכשיו תורכם להחליט שאתם רוצים להתחיל תהליך למידה והיכרות עם הגוף
              שלכם, בו נעבוד יחד כדי שתיהיו הגרסה הכי טובה של עצמכם.<br />
              יאללה, מחכה לכם!<br />
              <a class="contact-link unselectable" v-on:click="handleSendClick()"
                >שלחו לי הודעה</a
              >
              ונתחיל להתאמן 💪🏻💪🏻💪🏻
            </p>
          </div>
        </div>
        <div class="col-lg-6">
            <img alt="עדי זהיר" class="about-image mt-12" src="../../assets/about.jpg" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  methods: {
    handleSendClick() {
      this.$emit("send-click");
    },
  },
};
</script>

<style scoped>

.about {
  direction: rtl;
}

.about::before {
  content: " ";
  background-color: #FFC400;
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  right: 0;
  background-image: url("../../assets/about-background.svg");
  background-size: cover;
  will-change: transform;
}
.about-text {
  font-size: 15px;
  line-height: 2;
  text-align: justify;
}

.about-image {
  width: 400px;
  border: 5px solid rgba(255, 255, 255, 0.2);
  border-radius: 20px;
  float: right;
  margin-right: calc(50% - 200px);
}

.contact-link {
  color: #007bff !important;
  cursor: pointer;
  text-decoration: none;
}
</style>
