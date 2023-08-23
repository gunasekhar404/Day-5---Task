# Day-5---Task

1) For the given JSON iterate over all for loops (for, for in, for of, forEach)

a) The ‘For’ Loop :
var divisions = JSONObject.division.division;

for (var i=0; i < divisions.length; i++) {
    // handle division of one team here,
    // don't need for loop if there only one team
    // just do division[i].team.id
    for (var j=0; j < divisions[i].length; j++) {
        var teamId = divisions[i].team[j].id;
        alert(teamId);
    }
}

b) The "For in" Loop :
var jsonObject = {
  name: 'Guna',
  Age: '23'
};

for (var prop in jsonObject) {
  alert("Key:" + prop);
  alert("Value:" + jsonObject[prop]);
}

c) The "For of" loop :
ar arr = [ {"id":"10", "class": "child-of-9"}, {"id":"11", "class": "child-of-10"}];
    
for (var i = 0; i < arr.length; i++){
  document.write("<br><br>array index: " + i);
  var obj = arr[i];
  for (var key in obj){
    var value = obj[key];
    document.write("<br> - " + key + ": " + value);
  }
}

d) The "ForEach" loop :
var results = [ {"id":"10", "class": "child-of-9"}, {"id":"11", "classd": "child-of-10"} ];

results.forEach(function(item) {
    console.log(item);
});
