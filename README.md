# Query.am
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Հարց-պատասխան</title>
    <link rel="stylesheet" href="index.css" />
  </head>
  <body>
    <div class="testimonial-container">
      <div class="user">
        <img
          src="https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1"
          class="user-avater"
        />
        <div class="user-info">
          <h4 class="username">ProTanki</h4>
          <div class="twitter-handle"></div>
        </div>
      </div>
      <p class="testimonial">
        Բարի գալուստ ProTanki հարց-պատասխան կայք այստեղ ձեզ կտրվեն հարցեր դուք պետք է պատասխանեք իսկ եթե չգիտեք պատասխանը կարողեք անցնել մյուս հարցերին ցանկանումենք ձեզ հաճելի ժամանց ProTanki Online-ում.
      </p>
      <div class="line"></div>
    </div>

    <script src="index.js"></script>
  </body>
</html>

const testimonialsContainer = document.querySelector(".testimonial-container");
const testimonial = document.querySelector(".testimonial");
const userImage = document.querySelector(".user-avater");
const username = document.querySelector(".username");
const twitterHandle = document.querySelector(".twitter-handle");

const testimonials = [
  {
    name: "ProTanki",
    photo:
      "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: "ProTanki Online խաղում ինչու չեն ավելացնում XT Legacy Prime",
  },
  {
    name: "ProTanki",
    photo:
      "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: " Երբ է բացվել ProTanki Online Project-ը.",
  },
  {
    name: "ProTanki",
    photo:
      "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: " Ինչպիսի թարմացումներ կցանկանայք տեսնել ProTanki Online խաղում",
  },
  {
    name: "ProTanki",
    photo:
      "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: "ProTanki Online խաղի վերաբերյալ ինչ վիդեոներ կցանկանայք տեսնել armen5505 YouTube ալիքում",
  },
  {
    name: "ProTanki",
    photo:
      "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: "ProTanki Online խաղի վերաբերյալ որ YouTuber-ի վիդեոներնեք հավանում",
  },
  {
    name: "ProTanki",
    photo:
      "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: "Եթե չլինեյն խաղարկություներ արդյոք դուք կխաղայք ProTanki Online խաղը խնդրումեմ պատասխանել անկեխծ",
  },
  {
    name: "ProTanki",
    photo:
      "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: "ProTanki Online խաղում ով է առաջին  հայ XP/BP տուրնիռ խաղացողը",
  },
  {
    name: "ProTanki",
    photo:
       "https://sun9-65.userapi.com/s/v1/ig2/pnLXWi5wYmcjZOj7riOakoXQNnuvWRpALRD5oxSPRG1YXlnNctyM2-R1pFUJ1J4JUb1niY1aXjqEbqkojrexyq8c.jpg?size=200x200&quality=95&crop=0,0,1000,1000&ava=1",
    text: "ProTanki online  խաղում Shakal min ProFifa mega shakal min shakal shaft որ խաղարկության անունը չնշեցի"
  }
];

let counter = 1;

function showNextTestimonial() {
  const { name, position, photo, text } = testimonials[counter];

  testimonial.innerHTML = text;
  userImage.src = photo;
  username.innerHTML = name;
  twitterHandle.innerHTML = position;

  counter++;

  if (counter > testimonials.length - 1) {
    counter = 0;
  }
}

setInterval(showNextTestimonial, 10000);

* {
  box-sizing: border-box;
}

body {
  background: rgb(28, 28, 28);
  font-family: sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  overflow: hidden;
}

.testimonial-container {
  background-color: rgb(19, 19, 19);
  color: #fff;
  padding: 5rem 8rem;
  max-width: 800px;
  position: relative;
  box-shadow: 0 2px 4px 2px rgb(19, 19, 19);
}

.testimonial {
  line-height: 25px;
  text-align: center;
}

.user {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.user-avater {
  border-radius: 100px;
  height: 100px;
  width: 100px;
  object-fit: cover;
}

.user .user-info {
  margin-top: 10px;
  text-align: center;
}

.user .username {
  margin: 0;
}

.line {
  background: crimson;
  height: 4px;
  width: 100%;
  margin-top: 20px;
  animation: animation 10s linear infinite;
}

@keyframes animation {
  0% {
    transform: scaleX(0);
  }
}
