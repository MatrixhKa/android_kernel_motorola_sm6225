# Only include Motorola DTBs
ifeq ($(CONFIG_MMI_DEVICE_DTBS),y)
ifneq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
$(error Moto DT w/o overlay is undefined!!!)
endif

# Motorola Device Trees
dtbo-$(CONFIG_BATHENA_DTB) += \
        bengal-bathena-evt-overlay.dtbo \
        bengal-bathena-evt1-overlay.dtbo \
        bengal-bathena-dvt2-overlay.dtbo \
        bengal-bathena-pvt1-overlay.dtbo \
        bengal-bathena-evt1-sku3-overlay.dtbo

bengal-bathena-evt-overlay.dtbo-base := bengal-moto-base.dtb
bengal-bathena-evt1-overlay.dtbo-base := bengal-moto-base.dtb
bengal-bathena-dvt2-overlay.dtbo-base := bengal-moto-base.dtb
bengal-bathena-pvt1-overlay.dtbo-base := bengal-moto-base.dtb
bengal-bathena-evt1-sku3-overlay.dtbo-base := bengal-moto-base.dtb

dtbo-$(CONFIG_GUAM_DTB) += \
        bengal-guam-evt-overlay.dtbo \
        bengal-guam-dvt-overlay.dtbo \
        bengal-guam-dvt2-overlay.dtbo

bengal-guam-evt-overlay.dtbo-base := bengal-moto-base.dtb
bengal-guam-dvt-overlay.dtbo-base := bengal-moto-base.dtb
bengal-guam-dvt2-overlay.dtbo-base := bengal-moto-base.dtb

dtbo-$(CONFIG_GUAMP_DTB) += \
        bengal-guamp-evt-overlay.dtbo \
        bengal-guamp-dvt-overlay.dtbo \
        bengal-guamp-dvt2-sku3-overlay.dtbo \
        bengal-guamp-dvt2-sku4-overlay.dtbo \
        bengal-guamp-pvt-overlay.dtbo

bengal-guamp-evt-overlay.dtbo-base := bengal-moto-base.dtb
bengal-guamp-dvt-overlay.dtbo-base := bengal-moto-base.dtb
bengal-guamp-dvt2-sku3-overlay.dtbo-base := bengal-moto-base.dtb
bengal-guamp-dvt2-sku4-overlay.dtbo-base := bengal-moto-base.dtb
bengal-guamp-pvt-overlay.dtbo-base := bengal-moto-base.dtb

dtbo-$(CONFIG_GUAMNA_DTB) += \
        bengal-guamna-gwlc-evt-overlay.dtbo \
        bengal-guamna-evt-overlay.dtbo \
	bengal-guamna-gwlc-dvt2-overlay.dtbo \
	bengal-guamna-dvt2-overlay.dtbo

ifeq ($(CONFIG_HIGHMEM),y)
bengal-guamna-evt-overlay.dtbo-base := bengal-moto-low-ram-base-guamna.dtb
bengal-guamna-gwlc-evt-overlay.dtbo-base := bengal-moto-low-ram-base-guamna.dtb
bengal-guamna-dvt2-overlay.dtbo-base := bengal-moto-low-ram-base-guamna.dtb
bengal-guamna-gwlc-dvt2-overlay.dtbo-base := bengal-moto-low-ram-base-guamna.dtb
else
bengal-guamna-evt-overlay.dtbo-base := bengal-moto-base-guamna.dtb
bengal-guamna-gwlc-evt-overlay.dtbo-base := bengal-moto-base-guamna.dtb
bengal-guamna-dvt2-overlay.dtbo-base := bengal-moto-low-ram-base-guamna.dtb
bengal-guamna-gwlc-dvt2-overlay.dtbo-base := bengal-moto-low-ram-base-guamna.dtb
endif

dtbo-$(CONFIG_BORNEO_DTB) += \
        bengal-borneo-evb-overlay.dtbo \
        bengal-borneo-evt-overlay.dtbo \
        bengal-borneo-dvt1-overlay.dtbo \
        bengal-borneo-dvt2-overlay.dtbo

bengal-borneo-evb-overlay.dtbo-base := bengal-moto-base-borneo.dtb
bengal-borneo-evt-overlay.dtbo-base := bengal-moto-base-borneo.dtb
bengal-borneo-dvt1-overlay.dtbo-base := bengal-moto-base-borneo.dtb
bengal-borneo-dvt2-overlay.dtbo-base := bengal-moto-base-borneo.dtb

dtbo-$(CONFIG_CEBU_DTB) += \
        bengal-cebu-evt-overlay.dtbo

bengal-cebu-evt-overlay.dtbo-base := bengal-moto-base-cebu.dtb

dtbo-$(CONFIG_CAPRI_DTB) += \
        bengal-capri-evt-overlay.dtbo \
        bengal-capri-evt-sku5-overlay.dtbo \
        bengal-capri-dvt2-overlay.dtbo \
	bengal-capri-dvt2-sku5-overlay.dtbo

bengal-capri-evt-overlay.dtbo-base := bengal-moto-base.dtb
bengal-capri-evt-sku5-overlay.dtbo-base := bengal-moto-base.dtb
bengal-capri-dvt2-overlay.dtbo-base := bengal-moto-base.dtb
bengal-capri-dvt2-sku5-overlay.dtbo-base := bengal-moto-base.dtb

dtbo-$(CONFIG_CAPRIP_DTB) += \
        bengal-caprip-evt-overlay.dtbo \
	bengal-caprip-dvt2-overlay.dtbo

bengal-caprip-evt-overlay.dtbo-base := bengal-moto-base.dtb
bengal-caprip-dvt2-overlay.dtbo-base := bengal-moto-base.dtb

dtbo-$(CONFIG_RHODE_DTB) += \
        khaje-rhode-evt-overlay.dtbo \
        khaje-rhode-dvt-overlay.dtbo

khaje-rhode-evt-overlay.dtbo-base := khaje-moto-base.dtb
khaje-rhode-dvt-overlay.dtbo-base := khaje-moto-base.dtb

dtbo-$(CONFIG_HAWAO_DTB) += \
        khaje-hawao-evt-overlay.dtbo

khaje-hawao-evt-overlay.dtbo-base := khaje-moto-base.dtb

dtbo-$(CONFIG_DEVON_DTB) += \
        khaje-devon-evt-overlay.dtbo \
        khaje-devon-dvt2-overlay.dtbo \
        khaje-devon-pvt-overlay.dtbo

khaje-devon-evt-overlay.dtbo-base := khaje-moto-base.dtb
khaje-devon-dvt2-overlay.dtbo-base := khaje-moto-base.dtb
khaje-devon-pvt-overlay.dtbo-base := khaje-moto-base.dtb

else
ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
        dtbo-$(CONFIG_ARCH_BENGAL) += \
                bengal-rumi-overlay.dtbo \
                bengal-qrd-overlay.dtbo \
                bengal-idp-overlay.dtbo \
                bengal-idp-nopmi-overlay.dtbo \
                bengal-idp-usbc-overlay.dtbo \
                bengalp-idp-overlay.dtbo \
                bengal-idp-1gb-overlay.dtbo \
                bengal-idp-2gb-overlay.dtbo \
                bengal-idp-usbc-1gb-overlay.dtbo \
                bengal-idp-usbc-2gb-overlay.dtbo \
                bengal-iot-idp-overlay.dtbo \
                bengalp-iot-idp-overlay.dtbo \
                bengal-iot-idp-2gb-overlay.dtbo \
                bengal-iot-idp-usbc-2gb-overlay.dtbo \
                bengal-iot-idp-usbc-overlay.dtbo \
                bengalp-iot-idp-2gb-overlay.dtbo \
                bengalp-iot-idp-usbc-2gb-overlay.dtbo \
                bengalp-iot-idp-usbc-overlay.dtbo

bengal-rumi-overlay.dtbo-base := bengal.dtb
bengal-qrd-overlay.dtbo-base := bengal.dtb
bengal-idp-overlay.dtbo-base := bengal.dtb
bengal-idp-nopmi-overlay.dtbo-base := bengal.dtb
bengal-idp-usbc-overlay.dtbo-base := bengal.dtb
bengalp-idp-overlay.dtbo-base := bengalp.dtb
bengal-idp-1gb-overlay.dtbo-base := bengal-1gb.dtb
bengal-idp-2gb-overlay.dtbo-base := bengal-2gb.dtb
bengal-idp-usbc-1gb-overlay.dtbo-base := bengal-1gb.dtb
bengal-idp-usbc-2gb-overlay.dtbo-base := bengal-2gb.dtb
bengal-iot-idp-overlay.dtbo-base := bengal-iot.dtb
bengalp-iot-idp-overlay.dtbo-base := bengalp-iot.dtb
bengal-iot-idp-2gb-overlay.dtbo-base := bengal-iot-2gb.dtb
bengal-iot-idp-usbc-2gb-overlay.dtbo-base := bengal-iot-2gb.dtb
bengal-iot-idp-usbc-overlay.dtbo-base := bengal-iot.dtb
bengalp-iot-idp-2gb-overlay.dtbo-base := bengalp-iot-2gb.dtb
bengalp-iot-idp-usbc-2gb-overlay.dtbo-base := bengalp-iot-2gb.dtb
bengalp-iot-idp-usbc-overlay.dtbo-base := bengalp-iot.dtb
else
dtb-$(CONFIG_ARCH_BENGAL) += bengal-rumi.dtb \
                bengal-qrd.dtb \
		bengal-idp.dtb \
		bengal-idp-nopmi.dtb \
		bengal-idp-usbc.dtb \
		bengalp-idp.dtb \
		bengal-idp-1gb.dtb \
		bengal-idp-2gb.dtb \
		bengal-idp-usbc-1gb.dtb \
		bengal-idp-usbc-2gb.dtb \
		bengal-iot-idp.dtb \
		bengalp-iot-idp.dtb \
		bengal-iot-idp-2gb.dtb \
		bengal-iot-idp-usbc-2gb.dtb \
		bengal-iot-idp-usbc.dtb \
		bengalp-iot-idp-2gb.dtb \
		bengalp-iot-idp-usbc-2gb.dtb \
		bengalp-iot-idp-usbc.dtb \
		bengalp-iot-idp-2gb.dtb
endif

ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
        dtbo-$(CONFIG_ARCH_KHAJE) += \
		khaje-atp-overlay.dtbo \
		khaje-qrd-overlay.dtbo \
		khaje-qrd-hvdcp3p5-overlay.dtbo \
		khaje-qrd-nowcd9375-overlay.dtbo \
		khaje-qrd-nopmi-overlay.dtbo \
		khaje-idp-overlay.dtbo \
		khaje-idp-nopmi-overlay.dtbo \
		khaje-idp-usbc-overlay.dtbo \
		khaje-idp-pm8010-overlay.dtbo \
		khaje-idps-display-90hz-overlay.dtbo \
		khajep-atp-overlay.dtbo \
		khajep-qrd-overlay.dtbo \
		khajep-qrd-hvdcp3p5-overlay.dtbo \
		khajep-qrd-nowcd9375-overlay.dtbo \
		khajep-qrd-nopmi-overlay.dtbo \
		khajep-idp-overlay.dtbo \
		khajep-idp-nopmi-overlay.dtbo \
		khajep-idp-usbc-overlay.dtbo \
		khajep-idp-pm8010-overlay.dtbo \
		khajep-idps-display-90hz-overlay.dtbo \
		khajeq-atp-overlay.dtbo \
		khajeq-qrd-overlay.dtbo \
		khajeq-qrd-hvdcp3p5-overlay.dtbo \
		khajeq-qrd-nowcd9375-overlay.dtbo \
		khajeq-qrd-nopmi-overlay.dtbo \
		khajeq-idp-overlay.dtbo \
		khajeq-idp-nopmi-overlay.dtbo \
		khajeq-idp-usbc-overlay.dtbo \
		khajeq-idp-pm8010-overlay.dtbo \
		khajeq-idps-display-90hz-overlay.dtbo \
		khajeg-atp-overlay.dtbo \
		khajeg-qrd-overlay.dtbo \
		khajeg-qrd-hvdcp3p5-overlay.dtbo \
		khajeg-qrd-nowcd9375-overlay.dtbo \
		khajeg-qrd-nopmi-overlay.dtbo \
		khajeg-idp-overlay.dtbo \
		khajeg-idp-nopmi-overlay.dtbo \
		khajeg-idp-usbc-overlay.dtbo \
		khajeg-idp-pm8010-overlay.dtbo \
		khajeg-idps-display-90hz-overlay.dtbo

khaje-atp-overlay.dtbo-base := khaje.dtb
khaje-idp-overlay.dtbo-base := khaje.dtb
khaje-idp-nopmi-overlay.dtbo-base := khaje.dtb
khaje-idp-usbc-overlay.dtbo-base := khaje.dtb
khaje-idp-pm8010-overlay.dtbo-base := khaje.dtb
khaje-idps-display-90hz-overlay.dtbo-base := khaje.dtb
khaje-qrd-overlay.dtbo-base := khaje.dtb
khaje-qrd-hvdcp3p5-overlay.dtbo-base := khaje.dtb
khaje-qrd-nopmi-overlay.dtbo-base := khaje.dtb
khaje-qrd-nowcd9375-overlay.dtbo-base := khaje.dtb
khajep-atp-overlay.dtbo-base := khajep.dtb
khajep-idps-display-90hz-overlay.dtbo-base := khajep.dtb
khajep-idp-overlay.dtbo-base := khajep.dtb
khajep-idp-nopmi-overlay.dtbo-base := khajep.dtb
khajep-idp-usbc-overlay.dtbo-base := khajep.dtb
khajep-idp-pm8010-overlay.dtbo-base := khajep.dtb
khajep-qrd-overlay.dtbo-base := khajep.dtb
khajep-qrd-hvdcp3p5-overlay.dtbo-base := khajep.dtb
khajep-qrd-nowcd9375-overlay.dtbo-base := khajep.dtb
khajep-qrd-nopmi-overlay.dtbo-base := khajep.dtb
khajeq-atp-overlay.dtbo-base := khajeq.dtb
khajeq-qrd-overlay.dtbo-base := khajeq.dtb
khajeq-qrd-hvdcp3p5-overlay.dtbo-base := khajeq.dtb
khajeq-qrd-nowcd9375-overlay.dtbo-base := khajeq.dtb
khajeq-qrd-nopmi-overlay.dtbo-base := khajeq.dtb
khajeq-idps-display-90hz-overlay.dtbo-base := khajeq.dtb
khajeq-idp-overlay.dtbo-base := khajeq.dtb
khajeq-idp-nopmi-overlay.dtbo-base := khajeq.dtb
khajeq-idp-pm8010-overlay.dtbo-base := khajeq.dtb
khajeq-idp-usbc-overlay.dtbo-base := khajeq.dtb
khajeg-atp-overlay.dtbo-base := khajeg.dtb
khajeg-qrd-overlay.dtbo-base := khajeg.dtb
khajeg-qrd-hvdcp3p5-overlay.dtbo-base := khajeg.dtb
khajeg-qrd-nowcd9375-overlay.dtbo-base := khajeg.dtb
khajeg-qrd-nopmi-overlay.dtbo-base := khajeg.dtb
khajeg-idp-overlay.dtbo-base := khajeg.dtb
khajeg-idp-nopmi-overlay.dtbo-base := khajeg.dtb
khajeg-idp-pm8010-overlay.dtbo-base := khajeg.dtb
khajeg-idp-usbc-overlay.dtbo-base := khajeg.dtb
khajeg-idps-display-90hz-overlay.dtbo-base := khajeg.dtb
else
dtb-$(CONFIG_ARCH_KHAJE) += khaje-idp.dtb \
		khaje-qrd.dtb \
		khaje-qrd-hvdcp3p5.dtb \
		khaje-qrd-nowcd9375.dtb \
		khaje-idp-nopmi.dtb \
		khaje-idp-usbc.dtb \
		khaje-idp-pm8010.dtb \
		khaje-qrd-nopmi.dtb \
		khaje-idps-display-90hz.dtb \
		khaje-atp.dtb \
		khajep-atp.dtb \
		khajep-qrd.dtb \
		khajep-qrd-hvdcp3p5.dtb \
		khajep-idps-display-90hz.dtb \
		khajep-idp-nopmi.dtb \
		khajep-idp-usbc.dtb \
		khajep-idp-pm8010.dtb \
		khajep-qrd-nowcd9375.dtb \
		khajep-qrd-nopmi.dtb \
		khajeq-atp.dtb \
		khajeq-idps-display-90hz.dtb \
		khajeq-idp-nopmi.dtb \
		khajeq-idp-usbc.dtb \
		khajeq-idp-pm8010.dtb \
		khajeq-qrd.dtb \
		khajeq-qrd-nowcd9375.dtb \
		khajeq-qrd-hvdcp3p5.dtb \
		khajeq-qrd-nopmi.dtb \
		khajeg-atp.dtb \
		khajeg-qrd.dtb \
		khajeg-qrd-nowcd9375.dtb \
		khajeg-qrd-hvdcp3p5.dtb \
		khajeg-qrd-nopmi.dtb \
		khajeg-idp.dtb \
		khajeg-idp-nopmi.dtb \
		khajeg-idp-usbc.dtb \
		khajeg-idp-pm8010.dtb \
		khajeg-idps-display-90hz.dtb
endif

endif  # CONFIG_MMI_DEVICE_DTBS

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
