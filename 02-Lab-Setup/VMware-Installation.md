# VMware Installation

## Objective

Set up VMware Workstation to build a virtual enterprise environment for Active Directory administration.

## Why Virtualization?

-- Virtualization allows one physical computer to run multiple virtual computers simultaneously.
-- Imagine you have 1 physical laptop.
            laptop
               |
               |__windows 11  -- only runs one operationg system.
-- Now suppose you want:
        - windows server 2022.
        - windows 11.
        - kali linux.
        - ubuntu       
-- Instead of installing all four on the same laptop , virtualization allows you to run mulitple virtual computers simultaneously.Each 
one behaves like a separate computer.

    

## What is a Virtual Machine?

-- A Virtual Machine is a software-based computer.

It has its own:
        CPU
        RAM
        Hard Disk
        Network Adapter
        Operating System

Even though all of these are actually shared from the physical laptop.

examples: 
VM1 - DC01 ; OS - WINDOWS SERVER 2022 ; RAM - 4GB ; DISK - 60GB
VM2 - CLIENT1 ; OS - WINDOWS 11 ; RAM - 2GB ; DISK - 50GB

## What is a Hypervisor?
-- A Hypervisor is software that creates and manages Virtual Machines.

Examples:
    VMware Workstation
    Oracle VirtualBox
    Microsoft Hyper-V

                            Physical Laptop

                                    ↓

                            VMware Workstation

                                    ↓

                              DC01
                              CLIENT01
                              Kali Linux
    ### Here vmware workstation is the hypervisor....

## Why VMware?

-- Suppose tomorrow you accidentally destroy Active Directory.

Without VMware:
--Install Windows again.
With VMware:
--Restore Snapshot.

## Lab Environment

Host Operating System:
Windows 11

Hypervisor:
VMware Workstation

Virtual Machines:
- DC01
- CLIENT01

## Result

VMware was installed successfully and is ready for creating the virtual lab.