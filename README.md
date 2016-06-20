# Drupal 7 Module Threat Modeling

**..rough sketch ..  work in progress..**

This is a general workflow when creating a threat model for a Drupal 7 contrib
module.


##  Decompose the Module

- Make a threat model

  - What are the modules dependencies? Drupal, etc.

  - Does it except inputs; are there entry points for an attack?

  - Is secure information needed, ie User credentials/personal info

  - What permissions does the module operate under?


##  Determine and rank threats

- List found problems in code

  - What kind of breach is it?

  - Use STRIDE categorization
   
     - Spoofing
    
     - Tampering
    
     - Repudiation
    
     - Information Disclosure
    
     - Denial of Service
    
     - Elevation of Privilege.


-  Rank threats

  - Use DREAD model to determine risk
    
      - Score each from 1-10 and take average (1 low risk | 10 high risk)
    
         - Damage potential
        
         - Reproducibility
        
         - Exploitability
        
         - Affected users
        
         - Discoverability
    

##  Determine countermeasures and mitigation

- Determine what threats can be neutralized on our own

- Develop plan to fix threats, or notify the developer

  - Priorities, should we fix biggest or easiest to fix threats first?


