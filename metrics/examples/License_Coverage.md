## 1. Description
How much of the code base has declared licenses. This includes both software and documentation source files and is represented as a percentage of total coverage. 

## 2. Use Cases
License Coverage provides insight into the percentage of files in a software package that have a declared license, leading to two use cases: 
1. A software package is sourced for internal organizational use and declared license coverage can highlight points of interest or concern when using that software package. 
2. Further, a software package is provided to external, downstream projects and declared license coverage can make transparent license information needed for downstream integration, deployment, and use. 

**Note:** In both cases License Coverage less than 100% may require further investigation by distributors and consumers of a software package. 

## 3. Formula

## 4. Sample Filter and Visualization

### Web Presentation of DoSOCS2 Output: 
![](./images/licenses-declared-dosocs-1.png)

### JSON Presentation of DoSOCS2 Output: 
![](./images/licenses-declared-dosocs-2.png)

## 5. Sample Implementation
The above data was pulled from DoSOCSv2 and filtered through Jinja2 to get the desired information. Here is a sample of Jinja code to filter DoSOCSv2 code. The file that this implementation is inserted into may be found here:
https://github.com/DoSOCSv2/DoSOCSv2/blob/master/dosocs2/templates/2.0.tag
The code may be added to the end of the document. Run a “dosocs2 oneshot” scan and the new data will be at the end of the document. More information on DoSOCSv2 is found here:
https://github.com/DoSOCSv2/DoSOCSv2

```
{% set cnt = [0] %}
{% for file in package.files %}
{% if file.license_info[0].short_name != None %}
{% if cnt.append(cnt.pop() + 1) %}{% endif %}
{% endif %}
{% if loop.index == loop.length %}
TotalFiles: {{ loop.index }}
DeclaredLicenseFiles: {{ cnt[0] }}
PercentTotalLicenseCoverage: {{ '%0.2f' %  ((cnt[0] / loop.index) * 100) | float }}%
 {% endif %}
{% endfor %}

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
