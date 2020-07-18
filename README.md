# REGEX to transform .cfg to template 

Find: `^([a-zA-Z0-9_]+) \"(.*?)\"$`
Replace: `$1 "{{ sm_$1 | default('$2') }}"`
	
# TODO