---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=fwXEJh63sKc'
Speakers: [Tareque Hossain]
Tags: [django, django-forms]
ThumbnailUrl: 'http://i.ytimg.com/vi/fwXEJh63sKc/hqdefault.jpg'
Title: 'Django forms in a web API world'
date: '2012-09-05'
---
In our quest to modularize the architecture of web applications, we create
self-containing backend systems that provide web APIs for programmatic
interactions. This gives us the flexibility to separate different system
components. A system with multiple backend components e.g. user profile
engine, content engine, community engine, analytics engine may have a single
frontend application that fetches data from all of these components using
respective web APIs.

With the increased availability of powerful JavaScript frameworks, such
frontend applications are often purely JS based to decrease application
footprint, increase deployment flexibility and separate presentation from
data. The separation is very rewarding from a software engineering standpoint
but imposes several limitations on system design. Using django to construct
the API for arbitrary consumers comes with the limitation of not being able to
utilize the powerful django form subsystem to drive forms on these consumers.
But is there a way to overcome this restriction?

This is not a trivial problem to solve and there are only a few assumptions we
can make about the web API consumer. It can be a native mobile or desktop -
application or browser. We advocate that web APIs should provide sufficient
information about 'forms' so that they can be faithfully reproduced at the
consumer end.

Even in a API backend built using django, forms are essential for accepting,
filtering, processing and saving data. The django form subsystem provides many
useful features to accomplish these tasks. At the same time it facilitates the
process of rendering the form elements in a browser environment. The concepts
of form fields combined with widgets can go a long way in streamlining the
interface to interact with data.

We propose an architecture to serialize information about django forms (to
JSON) in a framework independent fashion so that it can be consumed by any
frontend application that renders HTML. Such information includes but is not
limited to basic form configurations, security tokens (if necessary),
rendering metadata and error handling instructions. We lovingly name this
architecture - django-remote-forms.

At WiserTogether, we are in the process of building a component based
architecture that strictly provides data endpoints for frontend applications
to consume. We are working towards developing our frontend application for web
browsers using backbone.js as MVC and handlebars as the templating engine.
django-remote-forms helps us streamline our data input interface with the
django forms living at the API backend.

In this talk we detail the architecture of our components, the mechanism of
delivering django form metadata over API and a backbone.js/ handlebars
implementation to consume the metadata and reproduce forms.
