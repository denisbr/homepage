Security, bugs & vulnerabilities
================================

* Rev. 2018-11-15 *phk*

.. toctree::
	:maxdepth: 1

	VSV00002.rst
	VSV00001.rst

We take security and quality *very* seriously in the Varnish project,
and we are more than a little proud that it took eleven years before
we had a major security issue.

I have found a security hole
----------------------------

Send email to phk@, my PGP key is at the bottom of this page.

I want to hear about security vulnerabilities
---------------------------------------------

Subscribe to the `Varnish Announce mailing list <https://www.varnish-cache.org/lists/mailman/listinfo/varnish-announce>`_

Vulnerabilities are and will also be listed further at the top of this page when they are new
and further down when they get older.

I'm a VIVU goddammit!
---------------------

Varnish users come in all sizes and importance, some are private
homepages, some are global CDNs, national governments or major
news outlets.

We want to provide some way to for Varnish users to get early warning about
future security incidents, but we do not want to pass judgement on
who are "Very Important Varnish Users" and much less to we want to
try to keep a list of up to date contact information for a list
that long.

We also don't want to make this information free, because if we
did, every criminal and his brother would sign up, to get a head
start against the Varnish users.

The rule going forward is therefore that if you contributed at least
EUR240 towards a `Varnish Moral License <http://phk.freebsd.dk/VML/>`_
in the 12 months previous to the disclosure-date, you will get early
warning about security issues.

On a case-by-case basis and purely at our discretion, we will also
extend this privilege to people who have contributed significantly
to the project in other ways.

Security Politics
-----------------

To be totally honest, this is section is quite speculative, we have
very little experience in this area, but this is how I expect we
would react to a major security issue:

* Assign a VSV number
* Try to get a CVE assigned.
* Create a VCL workaround, if at all possible.
* Fix the problem.
* If it makes sense (ie: no VCL workaround), roll a point-release.
* Announce on announce@varnish-cache.org and homepage.
* Kick ourselves, for *months*, for missing the bug.

Define "Major"
--------------

As you will notice if you peruse the CVEs listed below, we are not
kindly inclined to trophy-hunting and shrill alarmism.

If security advisories are to have any utility, they should be both
rare and relevant.

In particularly we do not consider it a security vulnerability that
somebody has a different taste in program architecture, or that
aliens might be able to DoS varnish servers if they have invented
quantum computers we cannot even comprehend.

On the other hand, if we find anything, on our own or thanks to
external contributors, which imperil Varnish users, we will not
hesitate to issue a CVE to get peoples attention.


11 years, really?
-----------------

Yes, indeed.  Luck probably has a lot to do with it, but luck tends
to favour the well-prepared, and we have had a big focus on quality
since the very start.

`Here is a piece I wrote about it last year <https://r.varnish-cache.org/docs/trunk/phk/thatslow.html>`_


List of all Varnish security issues
----------------------------------------

* CVE-____-____ -- :ref:`vsv00001`
* `CVE-2013-4484 -- < 3.0.5 -- DoS <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2013-4484>`_
* `CVE-2013-0345 -- <= 3.0.3 -- Local information leak <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2013-0345>`_
* `CVE-2009-4488 -- 2.0.6 -- Trophy hunting <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2009-4488>`_
* `CVE-2009-2936 -- < 2.1.0 -- Trophy hunting <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2009-2936>`_



PGP key
-------

Poul-Henning Kamp, author and main developer of Varnish::

 pub   4096R/0x8E5F44BA68E689C5 2013-09-28 [expires: 2018-09-27]
       Key fingerprint = 4357 5923 B8E1 1D70 3C66  5540 8E5F 44BA 68E6 89C5
 uid                 [ultimate] Poul-Henning Kamp <phk@FreeBSD.org>
 uid                 [ultimate] Poul-Henning Kamp <phk@phk.freebsd.dk>
 uid                 [ultimate] Poul-Henning Kamp <phk@ing.dk>
 uid                 [ultimate] Poul-Henning Kamp <phk@varnish.org>
 sub   4096R/0x1A605690A520ABD6 2013-09-28 [expires: 2018-09-27]

 -----BEGIN PGP PUBLIC KEY BLOCK-----
 Version: GnuPG v2.0.22 (FreeBSD)

 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
 =Bvkq
 -----END PGP PUBLIC KEY BLOCK-----

