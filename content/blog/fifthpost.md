---
title: Form Processing with The Coder's Guild
date: 2024-03-04
draft: false
tags:
  - Forms
  - Form Processing
  - HTML
  - The Coder's Guild
  - Bootstrap
---
<h1>Creating a HTML form, and adding it to our static site. </h1>

In this session we looked at how forms can be utilised on various websites and discussed the importance of safely collecting data, in line with GDPR. 

We also explored how to collect the data from our static sites and were tasked with doing so as our takeaway task. This session was a welcome respite from other heavy sessions we had been doing (this is not actually session 5, I've been tired since that hard hitting one).

For our takeaway task, we were asked to create a HTML form, stylise it with bootstrap and CSS and then to test the form on our static site and to test the data collected from it. 

Here is the form, please complete it so I can carry out the rest of the task 😉


    <h2>The Form</h2>
    <form action="#">
      <legend>
        <label for="name">Username:</label><br/>
        <input required type="text" id="name" name="name" placeholder="name" /><br/>
  
        <label for="email">Email:</label><br/>
        <input type="email" id="email" name="email" placeholder="a@a.com" /><br/>
  
        <label for="password">Password:</label><br/>
        <input
          type="password"
          id="password"
          name="password"
          pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}"
          title="Must contain at least one number and one uppercase and lowercase letter, and at least 8 or more characters"
          placeholder="Pa55word1"
        /><br/>
  
        <label for="tel">Telephone Number:</label><br/>
        <input type="tel" id="tel" name="tel" maxlength="11" /><br/>
  
        <label for="dob">Date of Birth:</label><br/>
        <input type="date" id="dob" name="dob" placeholder="01/01/2001" />
      </legend>

      <fieldset class="signup">
        <h3>Would you like to sign up?</h3>
        <input type="radio" id="signupYes" name="signup" value="Yes" />
        <label for="signupYes">Yes</label><br />
        <input type="radio" id="signupNo" name="signup" value="No" />
        <label for="signupNo">No</label><br />
      </fieldset>

      <label for="options">Coding expertise level:</label>
      <select id="options" name="options">
        <option value="1">Beginner</option>
        <option value="2">Intermediate</option>
        <option value="3">Expert</option>
        <option value="4">Other</option>
      </select>

      <input type="submit" class="submit" />
    </form>
