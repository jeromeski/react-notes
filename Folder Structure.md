src/
├── assets/
├── components/
│   
├── containers/
│   ├── App/
│   │    ├── components/
│   │    ├── meta/
│   │    ├── index.js
│   │    └── Loadable.js
│ {...}
├── content/
├── hooks/  
├── store/
├── utils/

Components folder
• contains all reusable components

Containers folder
• includes all modules 
  modules => contains the actual pages and it's logic 
• looks like a mini /src folder
• the components found inside this container is not used by other containers
• meta folder => mostly contains all the logic of the container

Utils
• contains common and global configurations and logic

Store
• contains redux store config


