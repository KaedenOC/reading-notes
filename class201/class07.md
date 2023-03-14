# Object-Oriented Programming, HTML Tables

## Domain Modeling

[Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling).

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders.

## HTML Tables

[HTML Tables](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics).

Layout tables reduce accessibility for visually impaired users: screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screen readers' output will be confusing to their users.

Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.

Tables are not automatically responsive: When you use proper layout containers (such as *header*, *section*, *article*, or *div*), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.
HTML tables should be used for tabular data

**Semantic** tables will include: th, tr, td.

## Constructors

[Constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors).

Define the "shape" of an object — the set of methods and the properties it can have — and then create as many objects as we like, just updating the values for the properties that are different.

Constructors, by convention, start with a capital letter and are named for the type of object they create.

Use constructors to create more than one object from a single object definition. the keyword **this** comes in handy when working with more than one object literal.