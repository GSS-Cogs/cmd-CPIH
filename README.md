# CMD CPIH

Script for tansforming CPIH data

Transform takes 1 input csv file, with the file name containing 'wda' and the input file is provided by the business area \n
Place the input file in the same directory as the script or alternatively change the location variable in CPIH_transform.ipynb to match the file location

1 output files is created
- v4-cpih.csv

The transform only works with the most recent months data, it then pulls the data of the previous publication from the CMD API and adds the most precent data to it.
Warning messages from the requests module is normal as "verify=False" is being used when making a request which is required when running this transform on network

The transform only requires use of base level packages
