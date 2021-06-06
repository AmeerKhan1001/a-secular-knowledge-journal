// Should be in head tag

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<style>

h2 {
color: #eda2fd;
}

h3 {
color: #b589d6;
}

@media only screen and (max-width: 767px) {
#buttonTierDiv, #buttonCategoryDiv, #buttonCommonDiv {
  position:relative;
  display:flex;
  flex-direction: row;
  flex-wrap:wrap;
  justify-content: space-around;
}
}

@media only screen and (min-width: 768px) {
#buttonTierDiv, #buttonCategoryDiv{
  position:relative;
  display:flex;
  flex-direction: row;
  flex-wrap:wrap;
  justify-content: space-between;
}
#buttonCommonDiv  {
position:relative;
display:flex;
flex-direction: row;
flex-wrap:wrap;
justify-content: space-around;
}
}

.tier {
  background-color: #fff;
  color: #242424;
  border: 2px solid;
  transition:0.5s ease-in-out;
  width: 220px;
  font-size: 20px;
  height: 50px;
  cursor: pointer;
  position: relative;
  margin: 0.5em;
}

.category {
  background-color: #fff;
  color: #242424;
  border: 2px solid;
  transition:0.5s ease-in-out;
  width: 220px;
  font-size: 20px;
  height: 50px;
  cursor: pointer;
  position: relative;
  margin: 0.5em;
}

@media only screen and (min-width: 1025px) {
.tier:hover, .tier.active:hover {
  color: #fff;
  background-color: #000;
  border-color: #eda2fd;
  box-shadow: 0 0em 0.8em 0.4em #eda2fd;
}

.category:hover, .category.active:hover {
  color: #fff;
  background-color: #000;
  border-color: #fde64b;
  box-shadow: 0 0em 0.8em 0.4em #fde64b;
}
}

.tier.active {
  color: #fdf;
  background-color: #000;
  border-color: #eda2fd;
  box-shadow: 0 0em 0.8em 0.05em #eda2fd;
}

.category.active {
  color: #fde64b;
  background-color: #000;
  border-color: #fde64b;
  box-shadow: 0 0em 0.8em 0.05em #fde64b;
}

</style>

// Should be before end of body tag

<script>

$("#btn1").click(function() {
  $("#mustDiv").toggle();
  $(this).toggleClass("active");
});

$("#btn2").click(function() {
  $("#favDiv").toggle();
  $(this).toggleClass("active");
});

$("#btn3").click(function() {
  $("#otherDiv").toggle();
  $(this).toggleClass("active");
});

$("#commonBtn").click(function() {
  $(".common").toggle();
  $(this).toggleClass("active");
});

$("#toolsBtn").click(function() {
  $(".tools").toggle();
  $(this).toggleClass("active");
});

$("#techBtn").click(function() {
  $(".tech").toggle();
  $(this).toggleClass("active");
});

$("#scienceBtn").click(function() {
  $(".science").toggle();
  $(this).toggleClass("active");
});

</script>
