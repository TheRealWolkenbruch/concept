# Entity Relationships

## Guardian

Table: guardians

User implemented with `RodaAuth`

**Attributes**:

```
Id Integer
Name String
Email email
Password String
Confimation String
```

### Ward

Table: wards

**Attributes**:

```
Id Integer
ContactData Text
Email email
f_guardian_id Integer
```

### BondSchedule

Table: bond_schedules

**Attributes**:

```
Id Integer
title text
headline text
Description String
starting_from DATETIME # "tricky to properly visualize in the GUI"
interval_hours Integer # the time in hours starting from RelevantTime until TIMEOUT
f_ward_id Integer
```

# Bond
Table: bonds

IF Time.Now() > valid_to AND seen_at IS NULL then alert(bond.bondschedule.ward.guardian.email)

**Attributes**:

```
id Integer
f_bond_id Integer
valid_from DATETIME
valid_to DATETIME
seen_at DATETIME DEFAULT NULL
how_do_you_feel SMALLINT
feedback_message TEXT
url_stub_id UUID UNIQUE # GET /bond/answer/:url_stub_id (-> seen_at: NOW()); POST $sameurl (-> fill feedback fields)
```
