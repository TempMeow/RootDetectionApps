# Root Beer's SE LINUX FLAG detection is false positive 
# CUSTOM ROM detection is ignorable
# Lineage package name overlay detection is ignorable
# These are false positive-

if (item.path.starts_with("/memfd:jit-cache") 
            item.path.starts_with("/dev/ashmem/jit-cache") 
            item.path.starts_with("/memfd:/jit-cache") 
            item.path.starts_with("/dev/ashmem//jit-cache") 
            item.path.starts_with("/dev/ashmem/dalvik-jit-code-cache") ||
            item.path == "[anon_shmem:dalvik-jit-code-cache]") {
