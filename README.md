

find . Find here
-maxdepth 1 Don't go into child directories
! -path . Exclude . / Current directory path
-type d match only directories
-print0 Separate output by null bytes \0
| xargs Pipe to xargs
-0 Input is null separated bytes
-I @@ Placeholder is @@. Replace @@ with input.
bash -c '...' Run Bash command
{...} Command grouping
&& Execute next command only if previous command exited successfully (exit 0)

Final ; is important, otherwise it will fail.

