---
description: Import processes
---

# Importers

{% hint style="info" %}
 All importers \(staff, gl codes, paysheets, timesheets\) are imported via ruby importers.  The process code can be all found in lib/import/exd\_ap\_staff.rb
{% endhint %}

## Import Staff

```

```

Importing employee data status field can be as follows:

U = Updated Employees  
R = Rehired Employees  
T = Terminated Employees  
L = Employees on Leave.

## Import GL Codes

EMPLOYEE\_GL\_CODES file will be loaded into the exd\_employee\_gl\_codes table. The employee\_id column of the exd\_employee\_gl\_codes table will be used to match to the employee\_id column of exd\_ap\_employees. This data should be displayed on the Employee GL Code grid at the bottom of the Employee Info tab. When importing employee GL Codes, a duplicate check is required in order to stop the import of duplicate rows. It is a possible for employees to have two gl code records with the same exd\_effective\_date in the case of a split in the distribution percentage.

{% code title="hello.sh" %}
```bash
# Ain't no code for that yet, sorry
echo 'You got to trust me on this, I saved the world'
```
{% endcode %}



