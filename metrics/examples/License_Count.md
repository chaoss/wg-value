## 1. Description

The total count of identified licenses in a software package where the same
license can be counted more than once if it is found in multiple source files.
This can include both software and document related licenses. This metric also
provides a binary indicator of whether or not the repository contains files
without license declarations.  

## 2. Use Cases

The most simple case for an IT Manager overseeing the acquisition and
management of open source software or an Open Source Program Office or
community manager delivering open source software to the marketplace is to have
a single license type declared across all files. This metric will illustrate
quickly and visible if there is one license or more than one; and the larger
the number, the more complex the considerations grow for decision makers. 

The second aspect of this metric is the binary indicator of whether or not the
repository (package) includes files that do not have license declarations. 

## 3. Formula

This metric is a "complexity of licensing case" flag for open source managers.
For example, the ideal case would look like the table below: 

| Number of Licenses | Files Without Licenses |
|--------------------|------------------------|
| 1                  | FALSE                  |

A more common case would require references to [Licenses
Declared](./License_Declared.md) and [License Coverage](./License_Coverage)
metrics, in the situation reflected in this table: 

| Number of Licenses | Files Without Licenses |
|--------------------|------------------------|
| 11                 | TRUE                   |

## 4. Sample Filter and Visualization
Does not apply in this case

## 5. Sample Implementation

A highly simplified version of the example provided in the [License
Declared](./License_Declared.md) metric. The following SQL will enumerate the
number of files with each license. The count of rows will indicate the number
of different licenses. The presence of a (NULL) row will indicate packages
without scanned license declarations. **Note** that its important to understand
that no file scanner is conclusive, especially if license declarations are not
in SPDX format. However, this metric still serves as a  high level indicator of
initial license risk when assessing packages (repositories) from this
perspective. 

```sql
SELECT
    concluded_license_id,
    COUNT ( * ) 
FROM
    packages_files 
WHERE
    package_id = 'package_id_of_package'
--- package_id is an int, but represented here as text for the purposes of explaining the abstraction. 
```

## 6. Known Implementations
1. Augur

## 7. Test Cases (Examples)

1. Available in the Augur test schema for these repositories: 
    - portable
    - openBSD
    - boringSSL

## 8. External References (Literature)
https://spdx.org/ 
https://www.fossology.org 

