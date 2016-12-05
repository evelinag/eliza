- title : Eliza tutorial
- description : Write your own therapist chatbot
- author : Evelina Gabasova
- theme : white
- transition : none

***

<img src="images/marvin.jpg" style="width:200px;float:left" />
<div style="margin-left:300px">

## Build your own 
# Chatbot therapist
## in F#

</div>

---

- data-background : images/slack-bots.png

<h1 style="font-size : 110pt;"> Chatbots </h1>

---

# What is a chatbot?

a) rule-based
<br/>
b) machine learning based

---

# Rule-based chatbot

Match predefined rules to user input

---

# Machine learning chatbot

I'm in **London** at **Progressive F# tutorials**.

---

# Plan for today

1. Build a rule-based chatbot locally.
2. Deploy to Azure.
3. Connect to Slack.
4. ...
5. Profit!

***

# Chatbot therapist

## Eliza

<img src="images/weizenbaum.jpg" style="width:200px;float:left" />
<div style="margin-left:300px">

1964 to 1966, MIT Artificial Intelligence Laboratory <br/>
## Joseph Weizenbaum

</div>

---

- data-background : black

[![](images/demo-eliza.png)](http://eliza-demo.azurewebsites.net/)

---

## How does Eliza work?

<table>
<tr>
  <td class="noborder"> <h3>Pattern</h3> </td>
  <td class="noborder"> <h3>Answers</h3> </td>
</tr>
<tr>
  <td class="noborder"></td>
  <td class="noborder"> Why do you need * ? </td>
</tr>
<tr>
  <td class="noborder"> I need * </td>
  <td class="noborder"> Would it really help you to get * ? </td>
</tr>
<tr>
  <td class="noborder"></td>
  <td class="noborder"> Are you sure you need * ? </td>
</tr>
</table>

---

## How does Eliza work?  🍰

<table>
<tr>
  <td class="noborder"> <h3>Pattern</h3> </td>
  <td class="noborder"> <h3>User input</h3> </td>
</tr>
<tr>
  <td class="noborder">I need *</td>
  <td class="noborder"> I need some cake </td>
</tr>
</table>

---

## How does Eliza work? 🍰

<table>
<tr>
  <td class="noborder"> <h3>User input</h3> </td>
  <td class="noborder"> <h3>Answers</h3> </td>
</tr>
<tr>
  <td class="noborder"></td>
  <td class="noborder"> Why do you need some cake? </td>
</tr>
<tr>
  <td class="noborder"> I need some cake </td>
  <td class="noborder"> Would it really help you to get some cake? </td>
</tr>
<tr>
  <td class="noborder"></td>
  <td class="noborder"> Are you sure you need some cake? </td>
</tr>
</table>

---

<table>
<tr>
  <td class="noborder"> <h3>Pattern</h3> </td>
  <td class="noborder"> <h3>User input</h3> </td>
</tr>
<tr>
  <td class="noborder">I need *</td>
  <td class="noborder"> I need some cake </td>
</tr>
</table>

<br/><br/>

<span class="fragment fade-in">
# Unification!

Find substitution that unifies two expressions
</span>

---

# The whole process 

1. Get user input
2. Find matching pattern
3. Extract substitution
4. Select answer and insert substitution
5. Reply to user

---

## What we're going to do:

1. Parse input into words and wildcards
2. Load data using Json type provider
3. Write unification
4. Insert substitution into answer and reply
5. Deploy locally
6. Deploy to Azure and use in Slack

****

# Link to slides

<div style="text-transform: lowercase; font-size: 72pt">

[evelinag.com/eliza](http://evelinag.com/eliza)

</div>

----

# Give me your email
## fseliza.slack.com
<br/>

[https://goo.gl/forms/weGhrcWi3nCRNUUB2](https://goo.gl/forms/weGhrcWi3nCRNUUB2)


---

# Download two github repositories

[github.com/evelinag/eliza-tutorial](https://github.com/evelinag/eliza-tutorial)

[github.com/evelinag/eliza-slack](https://github.com/evelinag/eliza-slack)

****

# Deploying to Azure

---

# The Deploy button

![](images/deploy-azure.png)

---

### Azure portal: Deployment options

![](images/deployment-options.png)

---

<img src="images/slack-logo.png" style="width=100px" />

# Integration

- Custom integration
- Slack App

---

# Custom integration

- Slash command
- Bot users - Real Time Messaging API
- App bot users - Real Time Messaging API, Events API

---

# Slack integration

### Slack commands

![](images/9_slack.png)

---

# Slack integration

[fseliza.slack.com](https://fseliza.slack.com/messages/general/)

---

<img src="images/1_slack.png" style="height:600px" />

---

![](images/2_slack.png)

---

![](images/3_slack.png)

---

![](images/4_slack.png)

---

![](images/5_slack.png)

---

![](images/6_slack.png)

---

![](images/7_slack.png)

---

![](images/8_slack.png)

---

![](images/9_slack.png)

****

# Learning more

<img src="images/weizenbaum-book.gif" style="width:300px;float:left" />
<div style="margin-left:350px">

- Dustin Moris Gorski: [Creating a Slack bot with F# and Suave in less than 5 minutes](https://dusted.codes/creating-a-slack-bot-with-fsharp-and-suave-in-less-than-5-minutes)

- [Custom integrations on Slack](https://api.slack.com/custom-integrations)

- Joseph Weizenbaum - Computer Power and Human Reason: From Judgment To Calculation.

</div>



