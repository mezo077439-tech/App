#!/usr/bin/env python3
"""
Script to extract New Folder.zip and commit contents to the repository
"""
import zipfile
import os

def extract_zip():
    zip_path = "New Folder.zip"
    extract_dir = "extracted_content"
    
    # Create extraction directory if it doesn't exist
    os.makedirs(extract_dir, exist_ok=True)
    
    # Extract the zip file
    print(f"Extracting {zip_path}...")
    try:
        with zipfile.ZipFile(zip_path, 'r') as zip_ref:
            zip_ref.extractall(extract_dir)
        print(f"Successfully extracted to {extract_dir}/")
        return True
    except Exception as e:
        print(f"Error extracting zip: {e}")
        return False

if __name__ == "__main__":
    extract_zip()
