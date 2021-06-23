
FAILED: out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy

/bin/bash -c "(ASAN_OPTIONS=detect_leaks=0 out/host/linux-x86/bin/checkpolicy -M -c 		30 -o out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy.tmp out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy.recovery.conf ) && (out/host/linux-x86/bin/sepolicy-analyze out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy.tmp permissive > out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy.permissivedomains ) && (if [ \"userdebug\" = \"user\" -a -s out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy.permissivedomains ]; then 		echo \"==========\" 1>&2; 		echo \"ERROR: permissive domains not allowed in user builds\" 1>&2; 		echo \"List of invalid domains:\" 1>&2; 		cat out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy.permissivedomains 1>&2; 		exit 1; 		fi ) && (mv out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy.tmp out/target/product/gtaxllte/obj/ETC/sepolicy.recovery_intermediates/sepolicy )"

device/samsung/gtaxllte/sepolicy/isolated_app.te:2:WARNING 'unrecognized character' at token '

' on line 61988:

allow isolated_app app_data_file:dir getattr;

#line 1 "device/samsung/gtaxllte/sepolicy/isolated_app.te"

device/samsung/gtaxllte/sepolicy/mediaextractor.te:2:WARNING 'unrecognized character' at token '

' on line 62197:

#line 1 "device/samsung/gtaxllte/sepolicy/mediaextractor.te"

allow mediaextractor fuse:file { getattr read };

device/samsung/gtaxllte/sepolicy/mediaextractor.te:3:WARNING 'unrecognized character' at token '

' on line 62198:

allow mediaextractor gpsd_exec:file getattr;

allow mediaextractor fuse:file { getattr read };

device/samsung/gtaxllte/sepolicy/mediaextractor.te:4:WARNING 'unrecognized character' at token '

' on line 62199:

allow mediaextractor gpsd_exec:file getattr;

device/samsung/gtaxllte/sepolicy/priv_app.te:2:WARNING 'unrecognized character' at token '

' on line 62321:

#line 1 "device/samsung/gtaxllte/sepolicy/priv_app.te"

allow priv_app su_exec:file { open read };

device/samsung/gtaxllte/sepolicy/priv_app.te:3:WARNING 'unrecognized character' at token '

' on line 62322:

allow priv_app device:dir open;

allow priv_app su_exec:file { open read };

device/samsung/gtaxllte/sepolicy/priv_app.te:4:WARNING 'unrecognized character' at token '

' on line 62323:

allow priv_app device:dir open;

allow priv_app proc_interrupts:file open;

device/samsung/gtaxllte/sepolicy/priv_app.te:5:WARNING 'unrecognized character' at token '

' on line 62324:

allow priv_app proc_modules:file { getattr open };

allow priv_app proc_interrupts:file open;

device/samsung/gtaxllte/sepolicy/priv_app.te:6:WARNING 'unrecognized character' at token '

' on line 62325:

allow priv_app proc_modules:file { getattr open };

allow priv_app sysfs:dir open;

device/samsung/gtaxllte/sepolicy/priv_app.te:7:WARNING 'unrecognized character' at token '

' on line 62326:

allow priv_app sysfs:file { getattr open read };

allow priv_app sysfs:dir open;

device/samsung/gtaxllte/sepolicy/priv_app.te:8:WARNING 'unrecognized character' at token '

' on line 62327:

allow priv_app sysfs:file { getattr open read };

allow priv_app proc_asound:dir search;

device/samsung/gtaxllte/sepolicy/priv_app.te:9:WARNING 'unrecognized character' at token '

' on line 62328:

allow priv_app proc_asound:file { open read getattr };

allow priv_app proc_asound:dir search;

device/samsung/gtaxllte/sepolicy/priv_app.te:10:WARNING 'unrecognized character' at token '

' on line 62329:

allow priv_app proc_asound:file { open read getattr };

allow priv_app system_data_file:dir { open read };

device/samsung/gtaxllte/sepolicy/priv_app.te:11:WARNING 'unrecognized character' at token '

' on line 62330:

allow priv_app adb_data_file:file { getattr open read execute };

allow priv_app system_data_file:dir { open read };

device/samsung/gtaxllte/sepolicy/priv_app.te:12:WARNING 'unrecognized character' at token '

' on line 62331:

allow priv_app adb_data_file:file { getattr open read execute };

allow priv_app adb_data_file:dir { getattr search };

device/samsung/gtaxllte/sepolicy/priv_app.te:13:WARNING 'unrecognized character' at token '

' on line 62332:

allow priv_app adb_data_file:dir { getattr search };

device/samsung/gtaxllte/sepolicy/property.te:11:WARNING 'unrecognized character' at token '

' on line 62343:

# rild

type rild_prop, property_type;allow radio system_app_data_file:dir getattr;

device/samsung/gtaxllte/sepolicy/property.te:13:WARNING 'unrecognized character' at token '

' on line 62345:

#line 2 "device/samsung/gtaxllte/sepolicy/radio.te"

allow radio adb_data_file:file { open read getattr };

device/samsung/gtaxllte/sepolicy/property.te:14:WARNING 'unrecognized character' at token '

' on line 62346:

allow radio gpu_service:service_manager find;

allow radio adb_data_file:file { open read getattr };

device/samsung/gtaxllte/sepolicy/property.te:15:WARNING 'unrecognized character' at token '

' on line 62347:

allow radio gpu_service:service_manager find;

allow radio gpuservice:binder call;

device/samsung/gtaxllte/sepolicy/property.te:16:WARNING 'unrecognized character' at token '

' on line 62348:

allow radio gpuservice:binder call;

device/samsung/gtaxllte/sepolicy/recovery.te:2:WARNING 'unrecognized character' at token '

' on line 62350:

allow recovery system_radio_prop:property_service set;

#line 1 "device/samsung/gtaxllte/sepolicy/recovery.te"

device/samsung/gtaxllte/sepolicy/shell.te:2:WARNING 'unrecognized character' at token '

' on line 62562:

allow shell bin_nv_data_efs_file:file getattr;

#line 1 "device/samsung/gtaxllte/sepolicy/shell.te"

device/samsung/gtaxllte/sepolicy/shell.te:3:WARNING 'unrecognized character' at token '

' on line 62563:

allow shell bin_nv_data_efs_file:file getattr;

allow shell efs_file:file getattr;

device/samsung/gtaxllte/sepolicy/shell.te:4:WARNING 'unrecognized character' at token '

' on line 62564:

allow shell hidl_base_hwservice:hwservice_manager add;

allow shell efs_file:file getattr;

device/samsung/gtaxllte/sepolicy/shell.te:5:WARNING 'unrecognized character' at token '

' on line 62565:

allow shell hidl_base_hwservice:hwservice_manager add;

allow shell sec_efs_file:file getattr;

device/samsung/gtaxllte/sepolicy/shell.te:6:WARNING 'unrecognized character' at token '

' on line 62566:

allow shell self:udp_socket ioctl;

allow shell sec_efs_file:file getattr;

device/samsung/gtaxllte/sepolicy/shell.te:7:WARNING 'unrecognized character' at token '

' on line 62567:

allow shell self:udp_socket ioctl;

allow shell sysfs:file { getattr open read };

device/samsung/gtaxllte/sepolicy/shell.te:8:WARNING 'unrecognized character' at token '

' on line 62568:

allow shell gpsd_exec:file getattr;

allow shell sysfs:file { getattr open read };

device/samsung/gtaxllte/sepolicy/shell.te:9:WARNING 'unrecognized character' at token '

' on line 62569:

allow shell gpsd_exec:file getattr;

allow shell kernel:system syslog_read;

device/samsung/gtaxllte/sepolicy/shell.te:10:WARNING 'unrecognized character' at token '

' on line 62570:

allow shell hal_telephony_hwservice:hwservice_manager add;

allow shell kernel:system syslog_read;

device/samsung/gtaxllte/sepolicy/shell.te:11:WARNING 'unrecognized character' at token '

' on line 62571:

allow shell hal_telephony_hwservice:hwservice_manager add;

allow shell mif_device:chr_file ioctl;

device/samsung/gtaxllte/sepolicy/shell.te:12:WARNING 'unrecognized character' at token '

' on line 62572:

allow shell radio_data_file:dir getattr;

allow shell mif_device:chr_file ioctl;

device/samsung/gtaxllte/sepolicy/shell.te:13:WARNING 'unrecognized character' at token '

' on line 62573:

allow shell radio_data_file:dir getattr;

allow shell rild_exec:file execute_no_trans;

device/samsung/gtaxllte/sepolicy/shell.te:14:WARNING 'unrecognized character' at token '

' on line 62574:

allow shell shell:udp_socket ioctl;

allow shell rild_exec:file execute_no_trans;

device/samsung/gtaxllte/sepolicy/shell.te:15:WARNING 'unrecognized character' at token '

' on line 62575:

allow shell shell:udp_socket ioctl;

device/samsung/gtaxllte/sepolicy/sswap.te:2:WARNING 'unrecognized character' at token '

' on line 62577:

#line 1 "device/samsung/gtaxllte/sepolicy/sswap.te"

type sswap, domain;

device/samsung/gtaxllte/sepolicy/sswap.te:3:WARNING 'unrecognized character' at token '

' on line 62578:

type sswap_exec, exec_type, file_type;

type sswap, domain;

device/samsung/gtaxllte/sepolicy/sswap.te:4:WARNING 'unrecognized character' at token '

' on line 62579:

type sswap_exec, exec_type, file_type;

device/samsung/gtaxllte/sepolicy/sswap.te:4:WARNING 'unrecognized character' at token '

' on line 62618:

#line 4

device/samsung/gtaxllte/sepolicy/sswap.te:5:WARNING 'unrecognized character' at token '

' on line 62619:

device/samsung/gtaxllte/sepolicy/sswap.te:6:WARNING 'unrecognized character' at token '

' on line 62620:

allow sswap sswap_data_file:file { create write open };

device/samsung/gtaxllte/sepolicy/sswap.te:7:WARNING 'unrecognized character' at token '

' on line 62621:

allow sswap sswap_data_file:file { create write open };

allow sswap sswap_data_file:blk_file { open read write };

device/samsung/gtaxllte/sepolicy/sswap.te:8:WARNING 'unrecognized character' at token '

' on line 62622:

allow sswap sswap_data_file:blk_file { open read write };

device/samsung/gtaxllte/sepolicy/sswap.te:9:WARNING 'unrecognized character' at token '

' on line 62623:

allow sswap init:unix_stream_socket connectto;

device/samsung/gtaxllte/sepolicy/sswap.te:10:WARNING 'unrecognized character' at token '

' on line 62624:

allow sswap property_socket:sock_file write;

allow sswap init:unix_stream_socket connectto;

device/samsung/gtaxllte/sepolicy/sswap.te:11:WARNING 'unrecognized character' at token '

' on line 62625:

allow sswap property_socket:sock_file write;

allow sswap sysfs:file { open write };

device/samsung/gtaxllte/sepolicy/sswap.te:12:WARNING 'unrecognized character' at token '

' on line 62626:

allow sswap system_prop:property_service set;

allow sswap sysfs:file { open write };

device/samsung/gtaxllte/sepolicy/sswap.te:13:WARNING 'unrecognized character' at token '

' on line 62627:

allow sswap system_prop:property_service set;

allow sswap block_device:dir search;

device/samsung/gtaxllte/sepolicy/sswap.te:14:WARNING 'unrecognized character' at token '

' on line 62628:

allow sswap self:capability sys_admin;

allow sswap block_device:dir search;

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:3:WARNING 'unrecognized character' at token '

' on line 62631:

#Policy for start_hci_filter

type start_hci_filter, domain;

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:4:WARNING 'unrecognized character' at token '

' on line 62632:

type start_hci_filter_exec, exec_type, file_type;

type start_hci_filter, domain;

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:4:WARNING 'unrecognized character' at token '

' on line 62671:

#line 4

;

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:5:WARNING 'unrecognized character' at token '

' on line 62672:

;

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:6:WARNING 'unrecognized character' at token '

' on line 62673:

allow start_hci_filter self:capability { setuid setgid dac_override };

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:7:WARNING 'unrecognized character' at token '

' on line 62674:

allow start_hci_filter self:capability { setuid setgid dac_override };

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:8:WARNING 'unrecognized character' at token '

' on line 62675:

allow start_hci_filter proc_sysrq:file { { getattr open read ioctl lock map watch watch_reads } { open append write lock map } };

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:9:WARNING 'unrecognized character' at token '

' on line 62676:

allow start_hci_filter ttyHS0_device:chr_file { { getattr open read ioctl lock map watch watch_reads } { open append write lock map } };

allow start_hci_filter proc_sysrq:file { { getattr open read ioctl lock map watch watch_reads } { open append write lock map } };

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:10:WARNING 'unrecognized character' at token '

' on line 62677:

allow start_hci_filter ttyHS0_device:chr_file { { getattr open read ioctl lock map watch watch_reads } { open append write lock map } };

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:11:WARNING 'unrecognized character' at token '

' on line 62678:

allow start_hci_filter uart_device:chr_file { open read write ioctl };

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:12:WARNING 'unrecognized character' at token '

' on line 62679:

allow start_hci_filter uart_device:chr_file { open read write ioctl };

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:14:WARNING 'unrecognized character' at token '

' on line 62699:

#line 14

device/samsung/gtaxllte/sepolicy/start_hci_filter.te:16:WARNING 'unrecognized character' at token '

' on line 62705:

#line 16

device/samsung/gtaxllte/sepolicy/toolbox.te:2:WARNING 'unrecognized character' at token '

' on line 62854:

allow toolbox init:fifo_file { getattr read write };

#line 1 "device/samsung/gtaxllte/sepolicy/toolbox.te"

device/samsung/gtaxllte/sepolicy/toolbox.te:3:WARNING 'unrecognized character' at token '

' on line 62855:

allow toolbox init:fifo_file { getattr read write };

allow toolbox init:unix_stream_socket { read write };

device/samsung/gtaxllte/sepolicy/toolbox.te:4:WARNING 'unrecognized character' at token '

' on line 62856:

allow toolbox system_data_file:file { read };

allow toolbox init:unix_stream_socket { read write };

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:2:WARNING 'unrecognized character' at token '

' on line 62900:

allow untrusted_app_25 mnt_media_rw_file:dir getattr;

#line 1 "device/samsung/gtaxllte/sepolicy/untrusted_app_25.te"

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:3:WARNING 'unrecognized character' at token '

' on line 62901:

allow untrusted_app_25 mnt_media_rw_file:dir getattr;

allow untrusted_app_25 proc:file getattr;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:4:WARNING 'unrecognized character' at token '

' on line 62902:

allow untrusted_app_25 proc_stat:file { getattr open };

allow untrusted_app_25 proc:file getattr;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:5:WARNING 'unrecognized character' at token '

' on line 62903:

allow untrusted_app_25 proc_stat:file { getattr open };

allow untrusted_app_25 gpsd_exec:file getattr;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:6:WARNING 'unrecognized character' at token '

' on line 62904:

allow untrusted_app_25 camera_device:dir search;

allow untrusted_app_25 gpsd_exec:file getattr;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:7:WARNING 'unrecognized character' at token '

' on line 62905:

allow untrusted_app_25 camera_device:dir search;

allow untrusted_app_25 camera_device:file { open read getattr };

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:8:WARNING 'unrecognized character' at token '

' on line 62906:

allow untrusted_app_25 serialno_prop:file { open read getattr };

allow untrusted_app_25 camera_device:file { open read getattr };

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:9:WARNING 'unrecognized character' at token '

' on line 62907:

allow untrusted_app_25 serialno_prop:file { open read getattr };

allow untrusted_app_25 proc_asound:dir search;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:10:WARNING 'unrecognized character' at token '

' on line 62908:

allow untrusted_app_25 proc_asound:file { open read getattr };

allow untrusted_app_25 proc_asound:dir search;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:11:WARNING 'unrecognized character' at token '

' on line 62909:

allow untrusted_app_25 proc_asound:file { open read getattr };

allow untrusted_app_25 adb_data_file:file { getattr open read execute };

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:12:WARNING 'unrecognized character' at token '

' on line 62910:

allow untrusted_app_25 adb_data_file:dir { getattr search };

allow untrusted_app_25 adb_data_file:file { getattr open read execute };

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:13:WARNING 'unrecognized character' at token '

' on line 62911:

allow untrusted_app_25 adb_data_file:dir { getattr search };

allow untrusted_app_25 proc_vmstat:file open;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:14:WARNING 'unrecognized character' at token '

' on line 62912:

allow untrusted_app_25 sysfs:file { getattr open read };

allow untrusted_app_25 proc_vmstat:file open;

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:15:WARNING 'unrecognized character' at token '

' on line 62913:

allow untrusted_app_25 sysfs:file { getattr open read };

allow untrusted_app_25 sysfs:dir { getattr open read };

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:16:WARNING 'unrecognized character' at token '

' on line 62914:

allow untrusted_app_25 proc_vmstat:file getattr;

allow untrusted_app_25 sysfs:dir { getattr open read };

device/samsung/gtaxllte/sepolicy/untrusted_app_25.te:17:WARNING 'unrecognized character' at token '

' on line 62915:

allow untrusted_app_25 proc_vmstat:file getattr;

device/samsung/gtaxllte/sepolicy/cbd.te:19:ERROR 'unknown type mif_device' at token ';' on line 61208:

# /dev/umts_boot0

allow cbd mif_device:chr_file { { getattr open read ioctl lock map watch watch_reads } { open append write lock map } };

checkpolicy:  error(s) encountered while parsing configuration

[  4% 897/19042] //external/selinux/secilc:secilc link secilc

[  4% 898/19042] //external/python/cpython3:py3-launcher-autorun link py3-launcher-autorun64 [linux_glibc]

[  4% 899/19042] build out/target/product/gtaxllte/obj/ETC/userdebug_plat_sepolicy.cil_intermediates/userdebug_plat_sepolicy.cil

[  4% 900/19042] build out/target/product/gtaxllte/obj/ETC/plat_sepolicy.cil_intermediates/plat_sepolicy.cil

[  4% 901/19042] //frameworks/ml/nn/runtime:libneuralnetworks link libneuralnetworks.so [arm apex30]

[  4% 902/19042] //packages/apps/Seedvault/libs/koin-android:seedvault-lib-koin-androidx-viewmodel aapt2 link [common]

[  4% 903/19042] //packages/apps/Seedvault/libs/koin-android:seedvault-lib-koin-android aapt2 link [common]

[  4% 904/19042] //frameworks/av/media/extractors/mpeg2:libmpeg2extractor link libmpeg2extractor.so [apex29]

[  4% 905/19042] //tools/security/sanitizer-status:sanitizer-status strip sanitizer-status

[  4% 906/19042] //frameworks/native/cmds/rss_hwm_reset:rss_hwm_reset strip rss_hwm_reset

[  4% 908/19042] //system/extras/tests/schedtest:schedtest strip schedtest

[  4% 909/19042] //system/vold:secdiscard strip secdiscard

[  4% 911/19042] //frameworks/ml/nn/runtime:libneuralnetworks link libneuralnetworks.so [apex30]

[  4% 912/19042] //system/core/run-as:run-as strip run-as

[  4% 913/19042] //external/openssh:scp strip scp

[  4% 914/19042] //system/core/sdcard:sdcard strip sdcard

[  4% 915/19042] //system/libhidl:libhidlbase strip libhidlbase.so

[  4% 917/19042] //system/core/fs_mgr:remount strip remount

[  4% 919/19042] //system/libhidl:libhidlbase strip libhidlbase.so

[  4% 920/19042] //frameworks/base:platformprotos javac [linux_glibc common]

ninja: build stopped: subcommand faile
