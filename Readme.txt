https://github.com/armory-io/arm



arm dinghy render dinghy_1 --modules ./examples/modules --rawdata ./examples/RawData.json --output ./testing

./arm-2.1.1-darwin-amd64 dinghy render ./examples/json/dinghyfile_globals --modules ./examples/json/modules --rawdata ./examples/RawData.json --output ./testing

./arm-2.1.1-darwin-amd64 dinghy render shaziyatest/dinghyfile_with_error  --output shaziyatest/output/dinghyfile_with_error_output

./arm-2.1.1-darwin-amd64 dinghy render shaziyatest/dinghyfile_simple --output shaziyatest/output/dinghyfile_simple_output

$ arm dinghy render ./examples/dinghyfile_globals --modules ./examples/modules --rawdata ./examples/RawData.json --output ./testing
INFO[2020-05-08 15:49:29] Checking dinghyfile                          
INFO[2020-05-08 15:49:29] Reading rawdata file                         
INFO[2020-05-08 15:49:29] Parsing rawdata json                         
INFO[2020-05-08 15:49:29] Parsing dinghyfile                           
INFO[2020-05-08 15:49:29] Parsed dinghyfile                            
INFO[2020-05-08 15:49:29] Output:                                      
{
  "application": "global_vars",
  "globals": {
    "waitTime": "42",
    "waitname": "default-name"
  },
  "pipelines": [
    {
      "application": "global_vars",
      "name": "Made By Armory Pipeline Templates",
      "stages": [
        {
          "name": "default-name",
          "waitTime": "42",
          "type": "wait"
        },
        {
          "name": "overwrite-name",
          "waitTime": "100",
          "type": "wait"
        }
      ]
    }
  ]
}
INFO[2020-05-08 15:49:29] Final dinghyfile is a valid JSON Object. 
