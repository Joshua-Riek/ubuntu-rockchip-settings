etc = get_option('sysconfdir')
var_lib = get_option('sharedstatedir')
usr_share = get_option('datadir')
sbin = get_option('sbindir')

install_data('server/99-fake-cloud.cfg',
             install_dir: etc / 'cloud/cloud.cfg.d')
install_data('server/getty-wait.conf',
             install_dir: etc / 'systemd/system/cloud-config.service.d')
install_data('server/override.conf',
             install_dir: etc / 'systemd/system/systemd-networkd-wait-online.service.d')

install_data('common/cpu-governor.service',
             install_dir: '/lib/systemd/system')
install_data('common/gpu-governor.service',
             install_dir: '/lib/systemd/system')
install_data('common/u-boot-menu.conf',
             install_dir: usr_share / 'u-boot-menu/conf.d')
install_data('common/rockchip-gzip.conf',
             install_dir: etc / 'initramfs-tools/conf.d')
install_data('common/rfkill.conf',
             install_dir: etc / 'modprobe.d')
install_data('common/9-rockchip-apparmor.conf',
             install_dir: etc / 'sysctl.d')
install_data('common/10-term.conf',
             install_dir: '/lib/systemd/system/serial-getty@.service.d')

install_data('desktop/mkswap.service',
             install_dir: '/lib/systemd/system')
install_data('desktop/swapfile.swap',
             install_dir: '/lib/systemd/system')
install_data('desktop/initial_preferences',
             install_dir: '/lib/chromium-browser')
install_data('desktop/plymouth',
             install_dir: etc / 'initramfs-tools/conf-hooks.d')
install_data('desktop/default',
             install_dir: etc / 'chromium-browser')
install_data('desktop/mimeapps.list',
             install_dir: usr_share / 'applications')
