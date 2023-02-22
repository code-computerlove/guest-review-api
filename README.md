# Guest Review API

_Thankyou for agreeing to take part in this practical assessment. Please feel free to use Google, refer to old repos, consult notes etc. Also, feel free to ask for clarification of any of the following, or to validate your understanding of the requirements._

Create a system for guests to leave reviews. Guest interactions should be through an ASP.NET Core Web API project.

We expect you to demonstrate:
- separation of concerns with separate projects for ASP.NET Core Web API, business logic etc.
- RESTful or other style of Web API (be prepared to justify choice)
- Programming principles
- TDD
- Mocking calls to database wrappers and external API wrappers

You will NOT need to demonstrate:
- MVC, Razor or Razor Pages
- Identity service, authentication or authorisation
- Database design
- Integration with external APIs

But we may ask questions on how such things might be implemented.

## Use case: Guest leaves review

### As a guest, I want to leave a review, so that other guests will be informed of my experience

Received customer reviews should contain a title (not empty; max 250 characters), body (not empty; max 500 characters) and a score between 1 and 5 inclusive.

E.G.
<table>
  <tr>
    <th>Title</th>
    <td>A fantastic time!</td>
  </tr>
  <tr>
    <th>Body</th>
    <td>Honestly best I've ever had. The whole family loved it</td>
  </tr>
  <tr>
    <th>Score</th>
    <td>5</td>
  </tr>
</table>

When customer reviews are received they should be validated and persisted. If a review fails validation, a suitable error response should be sent. Use a mock in place of the datastore. 

## Use case: Guest leaves a positive review

### As a marketeer, when a guest leaves a positive review (scoring 4 or 5), I want the review to be posted to social media, so that we broadcast the guest's positive experience

Use a mock in place of the social media façade.
