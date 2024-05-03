TOP=../..
include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE

#----------------------------------------------------
#  Optimization of db files using dbst (DEFAULT: NO)
#DB_OPT = YES

#----------------------------------------------------
# Create and install (or just install) into <top>/db
# databases, templates, substitutions like this
DB += motor.db
DB += asynComm.db
DB += asynCtrl.db
DB += motor_in_cs.template
DB += mpos.db
DB += pmacaux.db
DB += pmac_physical_limit.db
ifneq ($(RECCASTER),)
DB_INSTALLS += $(RECCASTER)/db/reccaster.db
endif

DB_INSTALLS += $(EPICS_BASE)/db/pmac_asyn_motor.db
DB_INSTALLS += $(EPICS_BASE)/db/motorstatus.db
DB_INSTALLS += $(EPICS_BASE)/db/pmacStatusAxis.db
DB_INSTALLS += $(EPICS_BASE)/db/pmacStatus.db
DB_INSTALLS += $(EPICS_BASE)/db/autohome.db
DB_INSTALLS += $(EPICS_BASE)/db/iocAdminSoft.db
DB_INSTALLS += $(EPICS_BASE)/db/save_restoreStatus.db
DB_INSTALLS += $(EPICS_BASE)/db/motorUtil.db

#----------------------------------------------------
# If <anyname>.db template is not named <anyname>*.template add
# <anyname>_template = <templatename>

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

