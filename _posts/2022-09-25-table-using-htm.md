---
toc: true
layout: post
description: Table using HTML and javascript fragments
categories: [Markdown, week-4]
title: Table using HTML and Javascript fragments
author: Aditya Ajay Nawnadhar
show_tags: true
comments: true
image: images/postimage5.png
---

# Making the table-

<table id="mine" style = "width:100%">
    <tr>
        <th>Countries</th>
        <th>Best food</th>
    </tr>
    <tr>
        <td rowspan="3">Korea</td>
        <td>Korean BBQ</td>
    </tr>
    <tr>
        <td>Kimchi</td>
    <tr>
        <td>Bibimbap</td>
    </tr>
    <tr>
        <td rowspan="3">Japan</td>
        <td>Sushi</td>
    </tr>
    <tr>
        <td>Tempura</td>
    <tr>
        <td>Udon</td>
    <tr>
        <td rowspan="3">China</td>
        <td>Fried Rice</td>
    </tr>
    <tr>
        <td>Kung Pao Chicken</td>
    <tr>
        <td>Dumplings</td>

<script>
function myFunction() {
  document.getElementById("mine").style.fontSize = "35px"; 
  document.getElementById("mine").style.color = "blue";
}
</script>

<center><button type="button" onclick="myFunction()" style="background: red">Click Me!</button></cente>

<script>
function person(name, role, class) {
    this.name = name;
    this.class = ghID;
    this.role = classOf;
}

var teammates = [
    new person("Arnav", "DevOps", "senior"),
    new person("Tay", "backend", "sophmore"),
    new person("Luke", "scrumleader", "senior"),
    new person("Aditya", "frontend", "junior")
]
person.prototype._toHtml = function() {
  // HTML Style is build using inline structure
  var style = (
    "display:inline-block;" +
    "border: 2px solid grey;" +
    "box-shadow: 0.8em 0.4em 0.4em grey;"
  );

  // HTML Body of Table is build as a series of concatenations (+=)
  var body = "";
  // Heading for Array Columns
  body += "<tr>";
  body += "<th><mark>" + "Name" + "</mark></th>";
  body += "<th><mark>" + "role" + "</mark></th>";
  body += "<th><mark>" + "Class" + "</mark></th>";
  body += "</tr>";
  // Data of Array, iterate through each row of compsci.classroom 
  for (var row of person) {
    // tr for each row, a new line
    body += "<tr>";
    // td for each column of data
    body += "<td>" + row.name + "</td>";
    body += "<td>" + row.role + "</td>";
    body += "<td>" + row.class + "</td>";
    // tr to end line
    body += "<tr>";
  }

   // Build and HTML fragment of div, table, table body
  return (
    "<div style='" + style + "'>" +
      "<table>" +
        body +
      "</table>" +
    "</div>"
  );

};