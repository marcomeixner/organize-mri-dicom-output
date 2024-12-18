# organize-mri-dicom-output
This script organizes the DICOM output of a Siemens MRI into subfolders according to SeriesNumber, SeriesDescription and StudyDate in the DICOM headers


Using dcmdump, this script organizes the output of a Siemens MRI (exported without creating a file System) into subfolders accroding to:

   - SeriesNumber (from dcm header)
   - SeriesDescription (from dcm header)
   - StudyDate (from dcm header)

input argument: a folder that contains one folder for each scan session at the scanner 
                 (exported as 'Erweitert' and without 'a Dicom file system')

output: one output folder is create for each individual combination of SeriesNumber, StudyDate and SeriesDescription