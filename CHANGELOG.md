Yii 2 Application Runtime Configuration extension Change Log
============================================================

1.0.7 under development
-----------------------

- Bug #17: Fixed `StorageActiveRecord` does not trigger ActiveRecord flow events (klimov-paul)
- Enh #18: Added options for customizing column names to `StorageDb` and `StorageActiveRecord` (inspirenmy, klimov-paul)


1.0.6, April 9, 2018
--------------------

- Enh #13: Added `Manager::$ignoreConfigureError` allowing to ignore config application errors (klimov-paul)


1.0.5, March 2, 2018
--------------------

- Chg: Version constraint for "yiisoft/yii2" is set to '~2.0.0' (klimov-paul)


1.0.4, February 6, 2017
-----------------------

- Enh: `Manager::configure()` allows to configure plain object not module only (klimov-paul)
- Enh: Added `Manager::getItemValue()` allowing to get particular item value (klimov-paul)
- Enh: Added `Manager::$autoRestoreValues` allowing to automatically restore item values from storage during manager initialization (klimov-paul)
- Enh: `Manager::$cacheId` can now be specified as a PHP callback (klimov-paul)
- Enh: Added `Item::$source` and `Manager::$source` allowing usage of the any object as config values source, not only current Yii application (klimov-paul)
- Enh: `Manager::$items` now can be specified as a PHP callback (klimov-paul)
- Enh #6: `StorageActiveRecord` now updates existing records instead of re-creating them during data saving (klimov-paul)
- Enh #9: `StorageFilterTrait` created providing ability to use single entity for multiple configuration storage at `StorageDb`, `StorageMongoDb` and `StorageActiveRecord` (klimov-paul)


1.0.3, January 11, 2017
-----------------------

- Bug: Fixed `Item::attributes()` returns incorrect attributes list (klimov-paul)
- Enh #7: `Item::$label` converted into virtual property, allowing its automatic generation from `Item::$id` value (nexen2, klimov-paul)
- Enh #8: Added ability to clear only single item value via `Manager::clearValue()` (klimov-paul)


1.0.2, June 3, 2016
-------------------

- Enh #4: `StoragePhp` now invalidates script file cache performed by 'OPCache' or 'APC' (klimov-paul)


1.0.1, April 25, 2016
---------------------

- Bug #1: Fixed `Manager::composeConfig()` triggers PHP Warning in case `items` contains only single element (klimov-paul)


1.0.0, December 29, 2015
------------------------

- Initial release.
