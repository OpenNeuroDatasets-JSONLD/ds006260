# README                                                                                                                      
              
## Authors
César E. Corona-González, Claudia Rebeca De Stefano-Ramos, Juan Pablo Rosado-Aíza, Fabiola R Gómez-Velázquez, David I. Ibarra-Zarate, Luz María Alonso-Valerdi

##  Contact person                                                                                                          
César E. Corona-González

 https://orcid.org/0000-0002-7680-2953

a00833959@tec.mx

## Project name
Psychophysiological data from Mexican children with learning difficulties who strengthen reading and math skills by assistive technology

## Year that the project ran
2023
                                                                                                                    
##  Brief overview of the tasks in the experiment                                                                           

The current dataset consists of psychometric and electrophysiological data from children with reading or math learning difficulties. These data were collected to evaluate improvements in reading or math skills resulting from using an online learning method called Smartick. 

The psychometric evaluations from children with reading difficulties encompassed: spelling tests, where 1) orthographic and 2) phonological errors were considered, 3) reading speed, expressed in words read per minute, and 4) reading comprehension, where multiple-choice questions were given to the children. The last 2 parameters were determined according to the [standards from the Ministry of Public Education](https://rarchivoszona33.files.wordpress.com/2012/10/manual_fomento.pdf) (Secretaría de Educación Pública in Spanish) in Mexico. On the other hand, group 2 assessments embraced: 1) an assessment of general mathematical knowledge, as well as 2) the hits percentage, and 3) reaction time from an arithmetical task. Additionally, selective attention and intelligence quotient (IQ) were also evaluated.

Then, individuals underwent an EEG experimental paradigm where two conditions were recorded: 1) a 3-minute eyes-open resting state and 2) performing either reading or mathematical activities. EEG recordings from the reading experiment consisted of reading a text aloud and then answering questions about the text. Alternatively, EEG recordings from the math experiment involved the solution of two blocks with 20 arithmetic operations (addition and subtraction). Subsequently, each child was randomly subcategorized as 1) the experimental group, who were asked to engage with Smartick for three months, and 2) the control group, who were not involved with the intervention. Once the 3-month period was over, every child was reassessed as described before.
                                                                                                    
##  Description of the contents of the dataset                                                                              

The dataset contains a total of 76 *subjects* **(sub-)**, where two study groups were assessed: 1) *reading difficulties* **(R)** and 2) *math difficulties* **(M)**. Then, each individual was subcategorized as *experimental subgroup* **(e)**, where children were compromised to engage with Smartick, or *control subgroup*  **(c)**, where they did not get involved with any intervention.

Every subject was followed up on for three months. During this period, each subject underwent two EEG sessions, representing the *PRE-intervention* **(ses-1)** and the *POST-intervention* **(ses-2)**. 

The EEG recordings from the reading difficulties group consisted of a *resting state condition* **(run-1)** and while performing *active reading and reading comprehension activities* **(run-2)**. On the other hand, EEG data from the math difficulties group was collected from a *resting state condition* **(run-1)** and when *solving two blocks of 20 arithmetic operations* **(run-2 and run-3)**. All EEG files were stored in .set format. The nomenclature and description from filenames are shown below:

| Nomenclature             |   Description              |
|--------------------------------  |---------------------------         | 
|              sub-                    |            Subject                   |
|                M                      |       Math group               |
|                R                       |    Reading group             |
|              c                          |    Control subgroup        |
|              e                          |  Experimental subgroup|
|              ses-1                   |    PRE-intervention  |
|              ses-2                   | POST-Intervention  |
|              run-1                  |  EEG for baseline     |
|              run-2                  |  EEG for reading activity, or the first block of math|
|              run-3                  |  EEG for the second block of math|

Example: the file *sub-Rc11_ses-1_task-SmartickDataset_run-2_eeg.set* is related to:
- The 11th subject from the reading difficulties group, control subgroup (sub-Rc11).
- EEG recording from the PRE-intervention (ses-1) while performing the reading activity (run-2)
    
                                                                                                                  
##  Independent variables                                                                                                   
- Study groups:
    + Reading difficulties
      * Control: children did not follow any intervention
      * Experimental: Children used the reading program of Smartick for 3 months
    + Math difficulties
        * Control: children did not follow any intervention
        * Experimental: Children used the math program of Smartick for 3 months
- Condition: 
    + PRE-intervention: first psychological and electroencephalographic evaluation
    + POST-intervention: second psychological and electroencephalographic evaluation
                                                               
##  Dependent variables                                                                                                     
- *Psychometric data from the reading difficulties group*:
   * Orthographic_ERR: number of orthographic errors.
   * Phonological_ERR: number of phonological errors.
   * Selective_Attention: score from the selective attention test.
   * Reading_Speed: reading speed in words per minute.
   * Comprehension: score on a reading comprehension task.
   * GROUP: C for the control group, E for the experimental group.
   * GENDER: M for male, F for Female.
   * AGE: age at the beginning of the study.
   * IQ: intelligence quotient.

- *Psychometric data from the math difficulties group*:
   * WRAT4: score from the WRAT-4 test.
   * hits: hits during the EEG acquisition [%].
   * RT: reaction time during the EEG acquisition [s].
   * Selective_Attention: score from the selective attention test.
   * GROUP: C for the control Group, E for the experimental group.
   * GENDER: M for male, F for female.
   * AGE: age at the beginning of the study.
   * IQ: intelligence quotient.      

**Psychometric data can be found in the *01_Psychometric_Data.xlsx* file**

- *Engagement percentage within Smartick (only for experimental group)*
    * These values represent the engagement percentage through Smartick. 
    * Students were asked to get involved with the online method for learning for 3 months, 5 days a week. 
    * Greater values than 100% denote participants who regularly logged in more than 5 days weekly.

**Engagement percentage be found in the *05_SessionEngagement.xlsx* file**

##  Methods                                                                                                                    
### Subjects                                                                                                                  
Seventy-six Mexican children between 7 and 13 years old were enrolled in this study. 

### Information about the recruitment procedure
The sample was recruited through non-profit foundations that support learning and foster care programs. 
                                                                                   
### Apparatus                                                                                                                 
g.USBamp RESEARCH amplifier
                                                                                                      
### Initial setup                                                                                                             
1. Explain the task to the participant.
2. Sign informed consent.
3. Set up electrodes.

### Task details                                                                                                              
The *stimuli* nested folder contains all stimuli employed in the EEG experiments. 

**Level 1**
- Math: Images used in the math experiment.​​​​​​​
- Reading: Images used in the reading experiment.

**Level 2**
- Math
    * POST_Operations: arithmetic operations from the POST-intervention.        
    * PRE_Operations: arithmetic operations from the PRE-intervention.
- Reading
    * POST_Reading1: text 1 and text-related comprehension questions from the POST-intervention.
    * POST_Reading2: text 2 and text-related comprehension questions from the POST-intervention.
    * POST_Reading3: text 3 and text-related comprehension questions from the POST-intervention.
    * PRE_Reading1: text 1 and text-related comprehension questions from the PRE-intervention.
    * PRE_Reading2: text 2 and text-related comprehension questions from the PRE-intervention.
    * PRE_Reading3: text 3 and text-related comprehension questions from the PRE-intervention.

**Level 3**
- Math
    * *Operation01.jpg* to *Operation20.jpg*: arithmetical operations solved during the first block of the math EEG experiment.
    * *Operation21.jpg* to *Operation40.jpg*: arithmetical operations solved during the second block of the math EEG experiment.
    * *Experiment_Start.jpeg*: start of the experiment.
    * *Experiment_End.jpeg*: end of the experiment.
    * *End_Block_1.jpeg*: break between blocks.

- Reading
    * Q1.png: first question.
    * Q2.png: second question.
    * Q3.png: third question.
    * Reading1, Reading2, or Reading3: texts from the reading EEG experiment. 

**The files *3. Reading_Tags.xlsx* and *4. Math_Tags.xlsx* provide the following information:**
- Order: number for better event accommodation.
- Event: tag in EEG file.
- Subject: Subject identifier
- Intervention: PRE (ses-1) or POST (ses-2).
- Reading/Block: task identifier tag.
	* "R1", "R2", and "R3" indicates which reading was assigned to each participant.
	* "1" and "2" for the blocks of the math experiment. 
- Group: control or experimental.
- Description: event tag meaning.
- Question shown (PRE): There are no event tags for questions in the PRE-EEG. intervention. Question sequences were registered manually. 

### Experimental location                                                                                                     
Tecnologico de Monterrey. Av. Eugenio Garza Sada 2501 Sur, Tecnologico, 64849 Monterrey, N.L., Mexico.
                                                                          
### Missing data                                                                                                              
The file ***2. EEG Data Descriptor.xlsx*** describes the data availability for EEG recordings. Some cells are highlighted to indicate some situations:
- Yellow cells mean that the quality of the EEG signals is inconsistent. However, EEG files were included for EEG preprocessing purposes. Additionally, EEG events for these files were not exported.
- Red cells imply that data is unavailable due to technical problems during the experiment's run and saving.                                                                                    

### Notes                                                                                                                     
EEG signals were filtered online with a 0.1-100 Hz bandpass filter.
The electrode O2 showed technical issues during the EEG experiment. The authors suggest the interpolation of this electrode
                                                                           