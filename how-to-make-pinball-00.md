# Part 0: Introduction and buying materials

## Table of Contents
---
1. [Introduction](#Introduction)
1. [Gear, Equipment, and Material](#Gear,-Equipment,-and-Material)
1. [Steps](#Steps)
1. [Conclusion](#Conclusion)


## Introduction
---

There are many ways to accomplish building a pinball machine, and I initially tried writing out different choices of materials and gear to buy with different accompanying steps. However, it got too complicated to keep in a manageable "how to" format. I will perhaps modify this article in the future, but for now it will be close to the steps that I've personally done , rather than all the possible ways this can be done.

If you want to buy more material than is listed here, check this page for all of the gear and material, as well as what article it is needed for. Each tutorial will try to be as short as possible, so you might want to read ahead and buy materials in advance so you can keep working though them

These guides will utilize FAST pinball hardware and MPF (Mission Pinball Framework) for code.  



Each article will have:
 - An Introduction
 - A list of Gear, Equipment, and Materials that will be used in the article, and typically mark which pieces of equipment are newly introduced and which have been introduced before. 
 - A list of steps
 - Any background educational material that is needed for those unfamiliar with certain concepts

And lasty, as a disclaimer, get ready to shell out $1000+ in cold hard cash for all the equipment and materials. Pinball machines are expensive.

## Gear, Equipment, and Material:
---
- ### Wire (18 AWG) Stranded
    - Purpose: May be obvious, but electricity will flow through them. [Kind of...](https://www.youtube.com/watch?v=bHIhgxav9LY)
    - Get A LOT of wire as you will run out of wire faster than you think. 100 ft of each might be a good starting point.
    - Colors:
        - Black
        - White
        - Green
        - Red
        - Yellow
        - Blue
    - Link: https://bulkwire.com/stranded-hookup-wire-300volt-ul1007
    - **Note**: I recommend getting the PVC insulation. The reason is that later on, you will crimp and put pins into computer board pin housing, and I've personally had an easier time working with the PVCs to push them into the housing than other isulation materials like silicon. However, silicon is softer and might be easier to manage when your rat nest grows. It really doesn't matter what insulation material you have really
    - **Another note**: While you are buying this wire, you can order additional colors if you like. They'll surely come in handy one day




- ### Wire stripper
    - Purpose: Used for stripping the insulation off of the wires and revealing the copper inside. The copper will connect to other components, or other wire.

    - There are many kinds of wire strippers, but I highly recommend getting one similar to this: https://www.amazon.com/Stripper-Electrical-Klein-Tools-11063W/dp/B00BC39YFQ/ref=sr_1_6?crid=1B9ZEAE13XHF9&keywords=wire+strippers&qid=1639944928&sprefix=wire+strippers%2Caps%2C101&sr=8-6
    
- ### Multimeter (Optional, but highly recommended)
    - Purpose: Obtaining information about electrical components or circuits
    - Not needed immediately, but I definitely recommend getting one and will reference using it in the following articles
    - Link: https://www.lowes.com/pd/IDEAL-ID-600-Volt-Auto-Range-Multimeter/5000045535
    - **Note:** Enthusiasts seem to say that the Fluke brand is the ultimate multimeter, so maybe consider that - they can get pricey though.
    

- ### 8 Amp Slow blow fuses / MDL fuses / Time-delay fuses
    - Purpose: Protects you and the components in the circuit. If too much current flows through the a fuse, it will break, and thus break the circuit. 
    - Too much current can flow through the system during power spikes for example.
    - Slow blow means that the amount of current passing through the circuit must exceed the amperage rating for a specified time duration before it blows. Fast acting fuses, on the other hand will blow almost immediately. A slow blow or fast acting fuse should be chosen based on how frequent power spikes may be in your application, and to how critical they can be. For example, a slight spike over the amperage rating might not cause any damage if just on for a short amount of time.
    - More details about fuses can be found here: https://components101.com/articles/choosing-between-slow-blow-and-fast-blow-fuse-for-power-protection
    - Link: https://www.amazon.com/gp/product/B07GFGQGRV/ref=ppx_yo_dt_b_search_asin_image?ie=UTF8&psc=1

    
    
    - Some more notes on fuses from other pinball makers on choosing an amperage to use:
        > In a nut shell, 8A would be typical for 120V circuit, and 5A for 220/230V circuit for European applications 
        > 

        > For sure lower is better.  Too little even though it may not blow right away, may eventually get metal fatigue (from in-rush).
        >


        > I've been using a 4 amp fast blow fuse on the main line and it hasn't blown yet. 
        > 
        
        > Ive seen about a 3a draw typically when measured on pins. A 4 or 5a fuse seems reasonable— I think sterns might use a 5a? Not that 8a isn’t ok too, but I think you could go lower
        > 
- ### Fuse Holder:
    - Purpose: To enclose and hold the fuse
    - Link: https://www.amazon.com/gp/your-account/order-history/ref=ppx_yo_dt_b_search_od?ie=UTF8&ij=&opt=ab&ref_=&search=112-7218553-0804265
    - Make sure whatever one you get is equal or higher than the fuses you have chosen in terms of amperage  
    
    - **Note:** There are other types of fuse holders. If you decide to buy one that is not enclosed, be sure to enclose this somehow because if you or something else conductive comes into contact with exposed metal on the circuit while the circuit is powered on, bad things will happen


- ### Extension cord with exposed wires
    - Purpose: One end plugs into AC outlet. The other ends are exposed so that you can easily hook them up to your PSU, which will likely have exposed lugs for attaching wires to.
    - Link: https://www.amazon.com/Bergen-Industries-Inc-PS915143-Appliance/dp/B07BQ8PY21/ref=sr_1_2?keywords=extension+cord+with+exposed+wire&qid=1639941711&sr=8-2
    - You might want a different length depending on your needs.
            
- ### Box Cutter (Optional)
    - Purpose: Able to cut the extension cord outer insulation so that the inner cords can be exposed. This is optional because you can also just connect another wire to the internal extension cord wires to extend the length of the line
    - This is optional because you can also connect other wires to the extension cord wires to increase the length.
    

    
- ### Wire caps:
    - Purpose: Temporary connections. Eventually you will want to solder and heat shrink to get a more permanant and stable connection, or use another proper connection method for connecting wires together. You may find these helpful throughout the articles, but I'll _try_ to avoid including them in steps.
    - Link: https://www.amazon.com/Bates-Assortment-Electrical-Connectors-Terminal/dp/B08QTYY4M9/ref=sr_1_3?keywords=wire+caps&qid=1639944104&sr=8-3
    - You can get these from your local home improvement or electrical store
    
- ### FAST Pinball starter bundle
    - Purpose: Bundles together starting material needed to solid state pinball machine in a modern way. Geared towards homebrewers.
    - Link: https://store.fastpinball.com/product/fast-starter-bundle-power/33?cs=true&cst=custom
    - Individual components:
        - FAST Nano Board
            - Purpose: Controls communication between I/O boards and whatever computer you use that will be running the actual code. Also controls LEDs on playfield.
        - FAST Power Filter Board
            -  Purpose: Stores power in capacitors, provides slots for protective fuses, and provides a mechanism to turn off high voltage power under certain circumstances.
            
        - LED controllers
            - Purpose: Connects to an LED that the nano can control
        - 48V (High Voltage) Power Supply Unit (PSU)
            - Purpose: Converts AC to DC. Delivers High Power for use in playfield devices. (Passed through the Power filter board)
            - The power supplies provided here are from the Meanwell brand and can be bought from other sources if out of stock.
        - 5V/12V switching PSU
            - Purpose: Can deliver 5V and 12V to Nano board. (Passed through the power filter board)
        - I/O boards
            - Purpose: Mainly receives input from switches and drives power to playfield devices. Communicates to nano board in a network via an ethernet cable. 
        - Connector + Pins Add-on (Highly recommended. You will need these eventually)
            - Purpose: Used for Wire-To-Board connections. They are inserted into connector headers/housings which are connected to pins on the various boards. 
            - .156" connector pin (Molex Pin 0008520113)
                - Alternative source if FAST is sold out: [Click here](https://www.digikey.com/en/products/detail/0008520113/WM2313-ND/172057?utm_medium=email&utm_source=oce&utm_campaign=4251_OCE21RT&utm_content=productdetail_US&utm_cid=663792&so=69357227&mkt_tok=MDI4LVNYSy01MDcAAAF8s_z-aLIhv5OOwhLiwW9MFjDH1y5yTjKgXU7baZfzX7emaaQEmVIR6E0TKt1Zicd3gLQuP3mSYq2XtFzsx6Pc_UQqLo7M6GdiMD8kGvI)
            - .100" connector pin (TE Connectivity AMP Connectors 1375819-1)
                - Alternative source if FAST is sold out: [Click here](https://www.digikey.com/en/products/detail/1375819-1/A100453CT-ND/2233146?utm_medium=email&utm_source=oce&utm_campaign=4251_OCE21RT&utm_content=productdetail_US&utm_cid=663792&so=69357227&mkt_tok=MDI4LVNYSy01MDcAAAF8s_z-aE1LatPJ9hSDXniG60v9h39LdjiL6vF4d5cMLstnMPXf8lbZgSyr5DoqFgcVmQt6jTwccqxyZBydpIdL46jN7Fmmb72i9cERtAY)
            - .156" Connector header
            - .100" Connector header
   
    - If this is out of stock, you can buy the components individually here: https://store.fastpinball.com/
    - If the FAST boards are out of stock, you're out of luck until they stock up
    - If the power supplies, pins, or pin housings are out of stock, you can always buy them from different suppliers as they are 3rd party components
    
    - **Note:** My advice is to buy a lot of extra pins and pin headers/housing as you may mess up attaching pins to wires at first and will want lots of spares. Pins are cheap so don't worry too much.

    

### Power Entry Module (Optional)
- Purpose: Exposes AC cord connection, a power switch, and typically comes with a fuse, or at least a place to put a fuse
- Instead of cutting up an exposed AC cord and connecting that manually to a fuse and PSU, this provides an easy way
- Eventually I will probably list this as not optional and adjust the guides to use this instead as its safer and easier.
- Some entry modules may require soldering
- If you go with this, don't buy the Exposed wire extension cord, box cutter, fuse holder. You won't need them

### AC Power Cord (Optional)
- Purpose: Used with entry module listed above
- It's likely the kind that you plug into a computer monitor for power.

## Steps:
---
1. Order all the gear and materials listed above
1. Wait
        

## Conclusion
---
- After a few more tutorials, we will actually get into setting up the PSUs and FAST boards. The reason I won't immediately jump into it is that the FAST products _may_ take a while to ship. In the meantime, we can  cover some much needed knowledge. There will be more parts to purchase, so read ahead
- Move on to the next tutorial, as we will go over soldering. It is needed for pinball making. The wires shouldn't take too long to arrive. If you are really jonesing to get started and need practice wire, pick some up at the local store. It doesn't matter what guage for practicing.
- While you wait for the gear to be delivered, watch some videos on electricity if you are unfamiliar with electrical engineering concepts or need to brush up on them from your high school or university classes of yester-year :)
    - I'm a big fan of Engineering Mindset's videos:
        - Here are some videos to get started but I recommend checking out their other videos as well as other channels' videos you find
            - https://www.youtube.com/watch?v=mc979OhitAg&list=PLWv9VM947MKjuqlJVp5m_Edf66SrFSHx2
            - https://www.youtube.com/watch?v=kcL2_D33k3o
            - https://www.youtube.com/watch?v=WhATjUHgzxQ
            - https://www.youtube.com/watch?v=8Posj4WMo0o
            - https://www.youtube.com/watch?v=P-W42tk-fWc
            - https://www.youtube.com/watch?v=w82aSjLuD_8
            - https://www.youtube.com/watch?v=X4EUwTwZ110

### Acknowledgements
- [thepinballroom youtube channel](https://www.youtube.com/channel/UCx8P46g5EkVZ_h3oFdfVfVA) was what led me to start building a pinball machine
- The Fast pinball crew and community: https://pinside.com/pinball/community/pinsiders/fastpinball 
    - Reach out to fast pinball/aaron davis for an invite to the Fast Slack organization if you begin your pinball making journey. The community provides a wealth of information and knowledge 
