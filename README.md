# Recipe-website

<!DOCTYPE html>
<head>
<script src="/assets/jquery.js"></script>
<link href='https://fonts.googleapis.com/css?family=Londrina+Shadow' rel='stylesheet' type='text/css'>
<style>
div {
  height: 200px;
  background-size: cover;
  position: relative;
  margin: 40px 0 0 0;
  border-radius: 12px;
}
h1 {
  font-family: 'Londrina Shadow', cursive;
  text-align: center;
  font-size: 75px;
  color: #aaaaaa;
  margin: 60px 0 0 0;
  background: url('https://www.thegraciouspantry.com/wp-content/uploads/2013/08/how-to-share-a-recipe-1-1.jpg');
  background-size: cover;   
}
h2 {
  text-align: center;
  color: #bbbbbb;
  margin: 0px 0 70px 0;
}
p {
  color: rgba(255,255,255,1);
  background: black;
  background: linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  background: -webkit-linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  background: -moz-linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  padding: 10px;
  line-height: 28px;
  text-align: justify;
  position: absolute;
  bottom: 0;
  margin: 0;
  height: 30px;
  transition: height .5s;
  -webkit-transition: height .5s;
  -moz-transition: height .5s;
}
small {
  opacity: 0;
}
.show-description p {
  height: 150px;
}
.show-description small {
  opacity: 1;
}
.first{
  background-image: url("http://www.ourbodybook.com/wp-content/uploads/2015/10/Potatoleeksoup-2-of-2.jpg");
}
.second{
  background-image: url("https://23209-presscdn-pagely.netdna-ssl.com/wp-content/uploads/2016/04/5MinuteAvocadoToastIMG_8273edit-340x340.jpg");
}
.dessert{
  background-image: url("https://natashaskitchen.com/wp-content/uploads/2016/03/30-Minute-Stir-Fry-Recipe-with-Chicken-and-Rice-Noodles-Healthy-and-so-delicious-Stir-Fry-with-rice-noodles-chicken-broccoli...-stirfryrecipe-13.jpg");
}
.price {
  float: right;
}
@media (max-width: 500px) {
  h1 {
    font-size: 50px;
    margin-top: 20px;
    line-height: 40px;
  }
  h2 {
    font-size: 20px;
    margin: 20px 0 30px 0;
  }
  div {
    margin: 20px 12px 0 12px;
  }
  p {
    font-size: 20px;
    line-height: 24px;
  }
  small {
    font-size: 16px;
  }
}
</style>
</head>
<body>
<header>
    <h1>Jess and Amy's Recipe Website</h1>
    <ul>
      <li><a href="#">About Us</a></li>
      <li><a href="#">Recipes</a></li>
      <li><a href="#">Add your own</a></li>
    </ul>
  </header>
  <article>
    <h2>About us</h2>
    <p>We are two students who love cooking and most importantly eating. Welcome to our website containing some of our favourite recipes - we'd love to hear some of yours!.</p>
    <button>Like</button>
  </article>
  <article>
    <h2>Recipes</h2>
    <p>.....</p>
    <button>Like</button>
  </article>
  <article>
    <h2>Add your own</h2>
    <p>.......</p>
    <button>Like</button>
  </article>
  <script>
    $("button").on("click", function() {
      alert("Clicked!");
    });
  </script>
<h1>Jess and Amy's Recipe Website</h1>
<h2>a must see for students</h2>
<div class="first">
  <p>Sweet potato and leek soup <span class="price"></span><br />
</p>
</div>
<div class="second">
  <p>Avocado toast <span class="price"></span><br />
</p>
</div>
  
<div class="dessert">
  <p>Stir fry <span class="price">$8</span><br />
  <small></p>
</div>
<script>
  $('div').on('click', function() {
      $(this).toggleClass('show-description');
  });
</script>
</body>
