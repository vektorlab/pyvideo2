---
Category: 'PyCon AU 2015'
Copyright: 'creativeCommon'
Language: 'English'
SourceUrl: 'https://www.youtube.com/watch?v=HhcotmeioT8'
Speakers: [Fraser Tweedale]
Tags: []
ThumbnailUrl: 'https://i.ytimg.com/vi/HhcotmeioT8/hqdefault.jpg'
Title: 'Integrating Django with Identity Management Systems'
date: '2015-08-04'
---
Most Django developers are familiar with authentication and
authorisation on the open web, but the requirements and technologies
used inside companies and large organisations are different:

- Identities and groups are probably stored in an external identity
  management system's directory rather than in an application's
  database tables.

- Authorisation decisions will be based on group membership and
  policies that are defined outside the application.

- Users may be expected or required to use a *single sign-on*
  technology such as Kerberos or SAML to authenticate to applications.

This talk will familiarise the audience with these technologies
and demonstrate how Django applications can be integrated
with an identity management system to meet business
requirements while providing a positive user experience.  Particular
technologies covered will include:

- FreeIPA: an open-source identity management solution, for defining
  users, groups and authorisation policies

- mod_auth_gssapi / mod_auth_kerb: Apache modules for Kerberos
  authentication

- mod_lookup_identity: Apache module to retrieve user information
  from a directory

The talk will conclude with discussion about upcoming Kerberos
features, techniques for dealing with multiple authentication
methods, and progress in making identity management integration
easier for Django developers.

People developing or deploying Django applications in business
environments or for large open source projects with centralised
identity management will get the most out of this talk.
