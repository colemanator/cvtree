cmake_minimum_required(VERSION 3.3)
project(cvtree)


set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")



set(SOURCE_FILES
        data/AcMNPV.faa
        data/AdhoNPV.faa
        data/AdorGV.faa
        data/AIHV_1.faa
        data/AMEV.faa
        data/APMiV.faa
        data/ASFV.faa
        data/AsGV.faa
        data/AtHV_3.faa
        data/ATV.faa
        data/BAdV_4.faa
        data/BAdV_A.faa
        data/BAdV_B.faa
        data/BmNPV.faa
        data/BoHV_1.faa
        data/BoHV_4.faa
        data/BoHV_5.faa
        data/BPSV.faa
        data/CAdV.faa
        data/CalHV_3.faa
        data/CcBV.faa
        data/CeHV_1.faa
        data/CeHV_15.faa
        data/CeHV_17.faa
        data/CeHV_2.faa
        data/CeHV_8.faa
        data/CfDeFNPV.faa
        data/CfMNPV.faa
        data/CHV_7.faa
        data/CMLV.faa
        data/CNPV.faa
        data/CpGV.faa
        data/CPXV.faa
        data/CrleGV.faa
        data/CuniNPV.faa
        data/DAdV_A.faa
        data/DPV.faa
        data/ECTV.faa
        data/EHV_1.faa
        data/EHV_2.faa
        data/EHV_4.faa
        improved.cpp
        data/list.txt)

add_executable(cvtree parallel.cpp)