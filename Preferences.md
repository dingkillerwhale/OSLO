# **Useful Preference Items**

  *Address1* | *Address2* | *Address3*    adr1/adr2/adr3

      used for the address field in element drawings. Each string may be up to 36 characters long

  **_CCL_auto_compile_**    ccac
      
      If on, CCL compiler will automatically run whenever a CCL command is saved from the OSLO text editor

  *Draw_ray_arrows*    drra 
      
      If on, arrwos will be drawn on ray segments
      
  **_Graphics_autoclear_**    gacl
      
      Determines whether graphics windows are automatically cleared when graphics commands are issued. **When off, the output from several graphics commands to be superimposed**

  **_Graphics_axes_**     grax 
  
      Determines whether axes are drawn in plots
      
  **_Graphics_black_and_white_**    gfbw
   
      If on, only black and white are used in graphics windows
      
  **_Graphics_labels_**    glab
   
      Determines whether graphics output contains annotation
      
  *Graphics_pen_sequence*    pens
  
      This array defines the sequence of pen colours used by commands
      
  *Graphics_pen_width*   penw
  
      This preference controls the width of lines in printed output and in graphics files produced by OSLO. 
      
  *Graphics_white_bkgnd*    gfwb
   
      Determines whether the background colour for the graphics windows is black or white. Off is black and On is white.
      
  *Lens_auto_open*    lauo
  
      If on,when OSLO is restarted, the lens file that was open during the previous session is reopened.
      
  **_Max_wavelengths_**   mwvl
  
      the maximum number of wavelengths that may be defiend for a lens
      
  *Open_lens_ss_with_file*    oswf
  
      If on, the Surface Data Spreadsheet will open when a lens is opened
      
  *Output_page_mode*    page
  
      If on, the first line of text output from each command appears at the top of the text output window.
      
  **_Output_text_**    outp
  
      If on, text output from OSLO commands appears in the text output window. If off, no text output and numberic output is saved in spreadsheet buffer
      
  **_Save_ASA_best_so_far_**    sabf
  
      If on, **Adaptive Simulated Annealing** algorithm will save the lens each time it finds a new best(lowest error function value) solution during the annealing processf
  
  *Surface_labels*    sflb
  
      If on, object surface, aperture stop sufrace and image surface will be labelled OBJ, AST and IMS in surface data spreadsheet and surface data listing
      
  **_Wavelength_default_**    wvld
  
      the defaults for the first three entries in the wavelengths set - element 0 is Wavelength 1 and element 1 is Wavelength 2 and so forth
      
      type: array of real
      
  **_Weight_default_**     wgtd
  
      default wavelength weights corresponding to the Wavelength_default preference array
      
      type: array of real


