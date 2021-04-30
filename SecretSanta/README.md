# Original Description

This is derived from a quiz posted on rubyquiz.com see: http://rubyquiz.com/quiz2.html. Don't forget to review the [Assessment Criteria](https://github.com/pdcal/CodeDojos) in the top level or this repo.

## Problem Description

Secret Santa is a game played by friends around the world to add a little mystery into seasonal gift giving.

To play secret santa:
 * All the participants names are placed in a hat
 * Names are drawn and allocated to other players
 * Gifts are bought and shared anonymously

Obviously, the problem with a random hat draw is you can get yourself - so lets solve this problem with software!

Here are some sample names:

<pre>
  Luke Skywalker   [luke@theforce.net]
  Leia Skywalker   [leia@therebellion.org]
  Toula Portokalos [toula@manhunter.org]
  Gus Portokalos   [gus@weareallfruit.net]
  Bruce Wayne      [bruce@imbatman.com]
  Virgil Brigman   [virgil@rigworkersunion.org]
  Lindsey Brigman  [lindsey@iseealiens.net]
</pre>

### Story 1

Allocating secret santas

    As a user
    When I pass a list of names in a file
    Secret santas are allocated

### Story 2

Families must be split up

    As a user
    When I allocate secret santas
    Santas are not paired when they are related

### Story 3 (Stretch goal - Front end)

Provide a web based front end for the service that allows users to add (and only add) names and email addresses. This solution does not need to preserve data, so on refreshing the page the list will be empty, ready to be used again. This could be hosted online if you wanted, or could run locally. 

    As a user
    When I go to a web page
    can add a secret santa participant to a list

### Story 4 (Stretch goal - Back end)

Provide an API that when called enables CRUD against a single secret santa list. The API does not need to have any kind of front end, it should be able to be interacted with directly via HTTP requests (sent via a tool such as Postman). This could be hosted online if you wanted, or could run locally. 

    As a user
    When I submit a CRUD request relating to a single secret santa participant
    The secret santa participant is updated appropriately

    As a user
    When I submit the right request
    The allocated list of secret santas is returned
