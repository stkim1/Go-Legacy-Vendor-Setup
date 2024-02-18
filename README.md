# Go Legacy (<1.14) Vendor (Dependency) Condensor + Cleanup

The idea behind this repository was to handle Go Legacy (<1.14) dependencies as **flat** and **specific** as it was possible.  

Back in the days, go vendors could have their own sub  dependencies which would result in duplicated sub dependencies and bloated `vendor` directory.  

The idea was to point a specific version or a commit hash to reduce the duplication into a single dependency so that go vendors could inter-dependent each other if necessary and the `vendor` directory could be leaner to manage.  

This would ultimately result in the main project with cleaner dependencies depot and easier dependency issue solving path. All these are now getting solved by the Go language team. 

The main language is `python` as it provides an easier path to handle strings. I'm uploading this for a future reference.  

## How to run sample dependency setup  
1. edit [earlybird-glide.yaml](asset/earlybird-glide.yaml)  
2. `pip install -r requirements.txt`  
3. `./setup_dep_env.sh`  
4. Now, we are good to go.  