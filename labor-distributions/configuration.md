---
description: EXD config
---

# Configuration

EXD configuration

module name: "Labor Distribution"

```
exd:
    user_roles: true
    update_user_email: true
    host: **IP ADDRESS** 
    user: wti
    password: TEST_PASSWORD
    import_path: /home/wti/files/exd
    export_path: /home/wti/files/exd/export
    import_staff_filename: "AP_EMPLOYEE.dat"
    import_glcodes_filename: "EMPLOYEE_GL_CODES.dat"
    import_paysheets_filename: "XXEXD_PAYSHEET_PS.dat"
    import_timesheets_filename: "XXEXD_TIMESHEET_WPX.dat"
    export_wells_filename: "XXEXD_WELLS_LOV.dat"
    export_company_wells_filename: "XXEXD_BASIN_WELLS.dat"
    export_afes_filename: "XXEXD_PROJ_LOV.dat"
    export_afe_budget_lines_filename: "XXEXD_TASK_LOV.dat"
    export_afe_budget_lines_info_filename: "XXEXD_PROJ_TASK_INFO.dat"
    export_cost_centers_filename: "XXEXD_OPER_UNIT_LOV.dat"
    export_exd_accounts_filename: "XXEXD_ACCTS_2PS.csv"
```

{% hint style="info" %}
if user\_roles is true, then the roles table will display the Staff ID column correlating to the imported employee data.
{% endhint %}

Host information is used to specify location when running import of staff, gl codes, paysheets and timesheets





