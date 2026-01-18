<!-- ---1----|----2----|----3----|----4----|----5----|----6----|----7----|--*>
     -->

# ODMJNI

## Preservation of the Java Native Interface bridge to ODMA

ODMJNI was an effort to provide ODMA access from Java applications.  The
project was abandoned when changes to the way Microsoft Office, especially
Word, altered the way that that the application GUI worked, confounding how
ODMA-interfaced document-management systems could produce pop-up dialogs
atop the Office application's window.

Preservation here is as a worked example of JNI usage and demonstration
how C and C++ Language can be used to access the COM-like interface supplied
by JNI.

There is no intention of developing ODMJNI further.  The current code is
incomplete and also obsolete, based on x86 and with no provision for an x64 world and whatever that means for today's Java Virtual Machines.

<!-- 0.0.2 2026-01-18T17:16Z Explain that this is moth-balled.
     0.0.1 2026-01-17T19:29Z Corrected name of project
     0.0.0 2026-01-17T17:03Z placeholder with ruler and clean MD Lint

                        *** end of README.md ***
     -->
