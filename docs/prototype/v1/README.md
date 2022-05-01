К сожалению, я был болен в конце неделе (2я привика пфайзером) - и не все успел сделать :(

Notes:
  - See the chart via [Lucid](https://lucid.app/lucidchart/c5b6957a-cf0b-4ad8-8035-5da5babd6364/edit?invitationId=inv_732145d6-3b4a-4d11-a6c3-e3617067849a&page=0_0#)
  - I assumed (for simplicity) that each Application (Task Tracker, Accounting, Analytics) has read & write DBs. And each Application has access to the read DB of any other Application while the write DB could be accessed by a related Application. So it's easy to share the date. Yet then I figured that this is a bad idea because schema updates will be a nightmare to pull off as all the services will be affected - but unfortunately, I already don't have time to fix it.
  - I'm not sure about naming events.
  - Analytics will have a separate Dashboard UI and Auth - yet currently all the views there are similar to Accounting so I omitted it in this chart because i'm short on time.
  - Each flow with a command is a standalone service. Some services re-use other services.
  - Each flow with command, results in a Business event.
