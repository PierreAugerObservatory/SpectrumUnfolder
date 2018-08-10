# SpectrumUnfolder
A C++ software tool for unfolding the Auger energy spectrum. It was developed within the Pierre Auger Observatory project and used in the Auger inclined spectrum paper. It is distributed for research use only under the GNU General Public License v3.0.

## **Credits**
If you use SpectrumUnfolder for your research, please acknowledge it in your papers by citing the following references:

* `S. Riggi et al., "On the unfolding of the inclined energy spectrum", Pierre Auger Internal GAP Note 2011-140 (2011)`
* `The Pierre Auger Collaboration, "Measurement of the cosmic ray spectrum above 4 × 10^18 eV using inclined events detected with the Pierre Auger Observatory", JCAP 08 (2015) 049`

or consider including me (`S. Riggi, INAF - Osservatorio Astrofisico di Catania, Via S. Sofia 78, I-95123, Catania, Italy`)
as a co-author on your publications.

## **Status**
This software is currently not actively maintained. At present only the forward-folder method is included. 
Gold and Bayes unfolders to be included.

## **Installation**  

### **Prerequisites**
Install the project mandatory dependencies:  
* ROOT [https://root.cern.ch/]

Make sure you have set the following environment variables to the external library installation dirs 
* ROOTSYS: set to ROOT installation prefix

NB: Modify Makefile CPPFLAGS and LDFLAGS in case the dependency tools cannot be found.

### **Build**
To build the project:

* Clone this repository into your local $SOURCE_DIR    
  ```git clone https://github.com/PierreAugerObservatory/CRSourceFitter.git $SOURCE_DIR```    
* In the project directory type:    
  ```make```  

Binaries will be placed in the bin/ directory and libraries in the lib/ directory.

### **Usage**
* ```SpectrumUnfolder --input=[path-to-inputfile] [--histoname=[data-histo-name]]```       
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```--input -  Input file name containing histogram to be read (.root)```     
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```--histoname - Name of histogram with spectrum data to be unfolded (default=RecSpectrum)```  
