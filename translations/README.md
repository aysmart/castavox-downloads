# Translations

The scripture packs Pulpitry and Castavox download, and the catalogue that
names them.

`catalogue.json` is what the applications fetch. It lists every translation on
offer with its language, its compressed size and a SHA-256 of the file as
published. The applications check that hash before a single verse reaches a
church's library: a pack that does not match is deleted rather than imported,
because the failure being guarded against is a Bible with something else in it.

Each pack is a gzipped TSV — book number, book, chapter, verse, text — of one
translation, between one and two megabytes.

Adding a translation here puts it in every church's list without an application
update. Regenerate the catalogue rather than editing it by hand; the hashes are
computed from the files, and one maintained by hand is one that is eventually
wrong.
