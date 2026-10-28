# Android Studio 	ools/adt/idea - Native Windows ARM64 Port

This repository contains the patch and modified packaging scripts to build and package **Android Studio** IDE distribution natively for **Windows 11 ARM64** (Snapdragon X Elite, Snapdragon X Plus, and other ARM64 Windows PCs).

## Upstream Target
- **Upstream Tag / Branch**: studio-rabbit1-release (	ools/adt/idea)
- **Base Commit**: 84efec3b

## Modifications Overview
- Configured native Windows ARM64 packaging targets in studio/BUILD and studio/studio.bzl.
- Enabled native Windows ARM64 binary bundling (studio64.exe, snotifier.exe, WinShellIntegrationBridge.dll, 
estarter.exe, WinProcessListHelper.exe).
- Updated plugin descriptors to allow execution on Windows ARM64 without architecture mismatches.

## Application
To apply the changes directly onto upstream AOSP 	ools/adt/idea:
`ash
git apply 0001-windows-arm64-studio-packaging.patch
`
