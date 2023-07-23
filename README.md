[![deploy](https://github.com/o365hq/o365hq.com/actions/workflows/main.yml/badge.svg)](https://github.com/o365hq/o365hq.com/actions/workflows/main.yml)

# o365hq.com

Microsoft's Gold Partner website based on Zola and hosted in Azure. 

```
                -------------------------                                                           -------------------------
                    AZURE KEYVAULT                                                                       
                   (to store our own                                                                       GITHUB REPO
                    certificate)                                                                        
                -------------------------                                                           -------------------------
                            |                                                                                   |
                            |                                                                                   |
                -------------------------               -------------------------                   -------------------------
                                                            AZURE STORAGE v2                          GITHUB ACTIONS 
>>>--------            AZURE CDN           ----------      (RA-GRS distributed       ----------      (spellcheck/linkscheck          
                                                            on West US,East US)                       build&deploy to Azure)
                -------------------------               -------------------------                   -------------------------
                            |                                                                                   |
                            |                                                                                   |
                -------------------------                                                           -------------------------

                        AZURE DNS                                                                             ZOLA  
                                                                                                        static site engine
                -------------------------                                                           -------------------------
```
