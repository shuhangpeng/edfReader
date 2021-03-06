## New in version 1.2.0

### 1 API change:

* The onset of annotation and of the startTime for data records has been corrected. The times are now relative to the start of the recording and not - as in an EDF+/BDF+ file - relative to the start time specified in the header. The 'onset' name in the recordStartTimes has been renamed to 'startTime' as well.

* The superfluous and confusion 'isRecordStart' element is removed from the 'annotations' data frame

### Other changes:

* Insignificant signal values for annotations signals are now replaced with NA values.

* An issue regarding reading a from-till period with no annotation signals resolved.

* R signal number added to signal objects

* Improved / revised rendering of the S3 print() or summary() functions

* improved read margin to avoid 'till' rounding errors, see the vignette for details 

* the vignette has been updated accordingly.

## New in version 1.1.2

* a minor bug in testFromTill.R has been corrected.

* some small improvements

## New in version 1.1.1

* a example of a plot function added to the vignette. 

## New in version 1.1.0

### 1 API change:

Within the annotations object in an ebfdAsignal object 'annotations' has been changed to 'annotation'
Reason: It contains only one annotation

### Other changes:

* support for EDF+ / BDF+ files with multiple annotation signals

* support for non unique labels

* support for TAL's with multiple annotations  

* support of sub second start info in first data record 

* revised S3 print and summary functions

* some issues with +D files resolved

* revised vignette
