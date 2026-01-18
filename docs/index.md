<!-- index.md 0.0.0                 UTF-8                         2026-01-18
     ----1----|----2----|----3----|----4----|----5----|----6----|----7----|--*
     source <https://github.com/orcmid/ODMJNI/blob/master/docs/index.md>
     published at <https://orcmid.github.io/ODMJNI/index.html>
     -->
# ODMJNI Preservation on GitHub

<table border="0" width="100%">
  <tr>
    <td width="72%" align="left">
       <img src="images/ODMdev-logo.gif">
    </td>
    <td width="27%" height="6" valign="middle" align="right">
          <b><code>
          <a href="../../" target="_top">orcmid.github.io</a>&gt;
          </code></b>
          <br />
          <a href="https://clustrmaps.com/site/1bw9w" title="Visit tracker">
                <img src="//www.clustrmaps.com/map_v2.png?d=3-2eQV4fOuelVHp_YtztZ0hl9Uj4ei9zLKw_nRgCgyM&cl=ffffff" />
          </a>
          <br />
          <b><code>
          <a href="./" target="_top">ODMJNI</a>&gt;
          </code></b>
          <br /><br />
          <b><code>
          <a href="index.html" target="_top">index.html</a>&gt;</code></b>
          <br />
          <small><small>
            0.0.0 2026-01-18T19:28Z<!-- MAINTAIN THIS MANUALLY -->
          </small></small>
    </td>
  </tr>
</table>

ODMJNI was a project to provide access to the Open Document Management
API (ODMA) middleware for integration of document management services
desktop functions with productivity applications.  The sweet spot was
support for the ODMA32 bridge in Microsoft Office Word.

The ODMA32 bridge was a DLL that provided a C Language API to clients,
and a COM x86 interface from registered document-management system
client services.

ODMJNI is an additional layer above the ODMA32 bridge to provide access
from Java-based desktop applications.  The way that was accomplished involves the Java Native Interface (JNI) and it is instructive in how
that adaptation was arranged.

ODMJNI uses a particular hack involving the Java methods passing pointers
around under the guise of integers.  This device depended on x86
pointers and none of ODMJNI is suitable in today's x64 world.

There is no intention of reviving ODMJNI, especially in the absence of
any ODMA64.  This preservation is here because the use of COM behind
the scenes (essentially between the Java classes and the native DLL) may
be instructive.  It also should be understood that JNI is now enough
different that the trick may no longer be feasible.

There is also an instructive provision of COM interfaces that can be
treated as either C++ interfaces or C Language structs with a vtable
pointer as the first member.  I confess that figuring out how I managed
that is the incentive for digging up this old code as I work on the
oMiser API as part of
[The Miser Project on GitHub](https://orcmid.github.io/miser).


----

Using a GitHub account, discuss ODMJNI topics in the
[Discussion section](https://github.com/orcmid/ODMJNI/discussions).  Propose
improvements and removal of defects in ODMJNI preservation documentation and
software in the [Issues section](https://github.com/orcmid/ODMJNI/issues).
There are unlikely
[projects](https://github.com/orcmid/ODMJNI/projects?query=is%3Aopen)
at this time.  For any security concerns, please consult the
[project security policy](https://github.com/orcmid/ODMJNI/security).

<!--
  0.0.0  2026-01-18T19:28Z Placeholder using Miser front page 0.6.2 as
         boilerplate.

               *** end of docs/index.md ***                           -->
