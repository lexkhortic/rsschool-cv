<img src="img/my-photo-circle.png" width="250"/>

# KHORT ALIAKSEI <br> Junior Java Developer

## LINKS TO PET PROJECTS
[Recipe In Your Pocket](https://github.com/lexkhortic/RecipeInYourPocket)

## ABOUT ME

I am honing the stack of technologies that I own, in the near future I plan to dive into Spring Security and RESTFull Web services. I work well both in a team and on my own. I lead an active lifestyle.

## CONTACTS
### Phone & email:
+375(44)591-55-14

khort97@mail.ru

### Social networks & messengers:
[<img src="img/telegram-logo.png" width="35"/>](https://t.me/lexkhortic) [<img src="img/linkedIn_color.svg" width="35"/>](https://linkedin.com/in/lexkhortic)  [<img src="img/github-color.svg" width="35"/>](https://github.com/lexkhortic)  [<img src="img/instagram-color.png" width="35"/>](https://instagram.com/lex_khortic97)

### Discord-server nickname:
Aliaksei Khort (@lexkhortic)

## SKILLS
* Java: java 8+, Spring, Spring boot, Thymeleaf, JSP, JDBC,  JPA,
Hibernate;
* Building tools: Maven;
* Testing: JUnit;
* VCS: Git;
* DMS: MySQL;
* Frontend: HTML, CSS, JS;
* English: Pre-Intermediate(reading and communication);
* Code examples(JAVA):
  ```
    //display owner details after login
    @GetMapping("/company/{owner_id}/{pharm_id}")
    public String enteredInAccount(Model model, @PathVariable long owner_id, @PathVariable long pharm_id) {
        Owner owner = ownerServices.findOwnerByID(owner_id);
        List<Pharmacy> pharmacies = owner.getPharmaciesList();
        model.addAttribute("ownerID", owner.getId());
        model.addAttribute("company_name", owner.getNameCompany());
        model.addAttribute("pharmacies", owner.getPharmaciesList().stream().sorted().collect(Collectors.toList()));

        if (pharmacies.isEmpty()) {
            model.addAttribute("pharmacy", null);
            model.addAttribute("medicines", null);
        } else {
            Pharmacy pharmacy = owner.getPharmaciesList()
                    .stream()
                    .filter(el -> el.getId() == pharm_id)
                    .findFirst()
                    .orElse(null);
            model.addAttribute("pharmacy",  pharmacy);
            assert pharmacy != null;
            model.addAttribute("medicines", pharmacy.getMedicinesList().stream().sorted().collect(Collectors.toList()));
        }
        return "owner";
    }
  ```

## EDUCATION
**Sukhoi State Technical University of Gomel (September 2014 - June 2019)** - Automation engineer in mechanical engineering

**Computer Academy "STEP" (April 2022 - April 2023)** - Junior Java Developer

Learned modules (368 academic hours): JAVA Core, FRONT-END technologies, Theory of Database, JAVA technologies for WEB-Applications.

## EXPERIENCE
* **Academic projects:**
  
  *Recipe In Your Pocket* - a web-application for finding medicines in pharmacies in the city of Minsk has been implemented, with the   ability to register your company and a network of pharmacies with medicines. [[Link to GitHub]](https://github.com/lexkhortic/RecipeInYourPocket)

* **LLC "Industrial engineering company" (November 2021 - present)** - Design engineer
  
  Responsibilities are related to the design, calculations of machines and mechanisms, maintaining and compiling design documentation.
  
* **CJSC "Soligorsk Institute for Resource Saving Problems" (July 2019 - November 2021)** - Design engineer

  Responsibilities are related to the design, calculations of machines and mechanisms, maintaining and compiling design documentation.