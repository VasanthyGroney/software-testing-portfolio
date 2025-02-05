### Scenario 3: Verify behavior when rating is submitted without feedback

**Submit rating without comments**  
As a user, I want to be able to rate the product without adding comments.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 4: Verify behavior when feedback contains prohibited language

**Submit feedback with offensive terms**  
As a user, I expect that offensive words in comments will be blocked.  
**Error:** Comments do not appear, but if I edit and retype them, they do appear.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 5: Verify that a user can edit an existing rating and/or comment

**Submit feedback and edit comment and stars**  
As a user, I expect to be able to edit my comments and ratings.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 10: Verify behavior when age input is left empty

**Verify the behavior when the age field is left empty**  
As a user, I want to check what happens when I leave the age field empty.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 11: Verify behavior with an invalid age format

**Verify the behavior when an invalid age format is entered**  
As a user, I want to see what happens when I enter an invalid age format.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 12: Verify free shipping eligibility for orders at the minimum threshold

**Verify free shipping eligibility for orders with a total of 20€**  
As a user, when I make purchases equal to 20 euros or more, I expect free shipping.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 13: Verify shipping charges for orders just below the threshold

**Verify shipping eligibility for orders with a total of 19.99€**  
As a user, I expect that when making purchases of 19.99 euros, free shipping will not be applied.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 14: Verify shipping charges for orders well below the threshold

**Verify shipping charges for orders with a total of 10€**  
As a user, when I have a total of 10 euros in my cart, I expect that I will not receive free shipping.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 15: Notify the user about eligibility for free shipping

**Notify user when order total reaches 50€**  
As a user, when I make purchases of 50 euros or more, I expect free shipping.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 16: Notify the user about eligibility for free shipping at a higher threshold

**Notify user when order total reaches 100€**  
As a user, when I make purchases of 100 euros or more, I expect free shipping.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|

### Scenario 17: Verify shipping fee updates correctly when items are removed from the cart

**Verify re-application of shipping fee when total drops below 20€**  
As a user, I expect the shipping fee to be applied again if I reduce my order total to less than 20 euros.  

| Step# | Action | Expected Outcome | OK/NOK | URL | Link to Issue |
|-------|--------|-----------------|--------|-----|---------------|
