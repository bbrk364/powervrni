## ToDo items/ideas

- \[optimization] leverage API-filtering in applicable `Get-vRNI*` cmdlets, so as to improve performance and flexibility (vs. getting each item until name matches retrieved item, for example)
- \[enhancement] improve `Connect-vRNIServer` experience:  if user specifies credential with username in UPN format (username@mydomain.com), glean domain info from username instead of making the additionally supply `-Domain` value (maybe default to gleaning `Domain` value from username if "@" in name, and change `-Domain` to a switch param for specifying `-UseLocalAuth` or something); would expect most enterprises that are using vRNI to enable LDAP auth, so that is probably a better default than `LOCAL` for domain considerations
