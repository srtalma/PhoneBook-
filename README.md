# PhoneBook-

#define a function that welecom the user and give him some options 
def welcome():
    entry =int (input(""""Welcom to Lama contact book
                     what would you like to do?:
                     
                     1- Display your exctiting contacts
                     2-creat a new contact
                     3- check an entry
                     4- delete an entry 
                     5- exit
                     enter your entry here"""))
    
    #close the function
    return entry

#define phoneBook function
def phonebook():
    
    #intitat a empty dictionary 
    
    contact={}
    
    # creat a loop to run the phoneBook continuesly
    while True:
        
        #call welcome function 
        #set entry variable  in welecom function 
        
        entry = welcome()
        
        #Create conditions for decision making ,for any option entered by the user
        
        if entry ==1:
            # Check if the contact dictionary is initially empty.
            #If it is not empty, Print the current contact list in the phonebook
            if bool(contact) !=False:
                
                for k,v in contact.item():
                    
                    print (k,'--->',v)
                    
                else:
                    #inform the user that It's empty 
                    print ('you have an empty phone book, Go back to the menu to add new contact')
                    
                    
            #Create decision making for the second entry
            
            
        elif entry ==2:
            #Request for a phone number and contact name.
            phone_number= input('Please enter the phone number')
            contact_name= input ('please enter the contact name, Enter in the format "FirstName,LastName' )
            
            
            #Check if the contact number already exists in the Phonebook
            #If it does not, update the current Phonebook
            
