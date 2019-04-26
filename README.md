# Folder picker

A directory picker for Flutter

## Usage

   ```dart
   import 'package:folder_picker/folder_picker.dart';

   Navigator.of(context).push<FolderPicker>(
      MaterialPageRoute(
         builder: (BuildContext context) {
            return FolderPicker(
               rootDirectory: externalDirectory, /// a [Directory] object
               action: (BuildContext context, Directory folder) {
                 print("PICKED FOLDER $folder");
               });
   }));
   ```