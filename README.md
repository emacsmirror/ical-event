ical-event
==========

Accept/Decline iCalendar appointment invitations from Gnus.
Sync iCalendar event invitations from Gnus to Org agenda.

Status
======

This code has been merged into Gnus and Emacs24 as `gnus-icalendar` and that's
where any further development or bugfixes will happen.

Setup
=====

    (add-to-list 'load-path "/path/to/ical-event")
    (require 'gnus-calendar)
    (gnus-calendar-setup)
    
    ;; to enable optional iCalendar->Org sync functionality
    ;; NOTE: both the capture file and the headline(s) inside must already exist
    (setq gnus-calendar-org-capture-file "~/org/agenda.org")
    (setq gnus-calendar-org-capture-headline '("Calendar"))
    (gnus-calendar-org-setup)


