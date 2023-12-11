<template>
  <Card>
    <div class="section-tittle">Experience</div>
    <div class="experience-container">
      <div class="experience">
        <div>
          <img
            class="company-logo"
            src="https://media.licdn.com/dms/image/C4E0BAQHaT0cdmSpKFg/company-logo_100_100/0/1673379477461/onthegoaccountants_logo?e=1710374400&v=beta&t=-0VSgi0dEWdCcHNdvX8rmput0A-Mn8Au4eR59YDkSrQ"
          />
        </div>
        <div>
          <div>
            <div class="experience-tittle">Client Finance Manager</div>
            <div class="experience-first-info">
              OnTheGo Accountants · Full-time
            </div>
            <div class="experience-second-info">
              Sep 2022 - Present · 1 yr 4 mos
            </div>
            <div class="experience-skills">
              <strong>Skills:</strong> VAT Returns · UK Corporation Tax ·
              External Communications · Accounts Production · Communication
            </div>
          </div>
        </div>
      </div>

      <div class="experience-divisor"></div>

      <div class="experience">
        <div>
          <img
            class="company-logo"
            src="https://media.licdn.com/dms/image/C4E0BAQHra1IWBElo3Q/company-logo_100_100/0/1631375729449/armstrongs_accountancy_limited_logo?e=1710374400&v=beta&t=XjzAS-J_szw47iNWUOabv-nd4ZNWo-zEkk3d4EtRJ6s"
          />
        </div>
        <div>
          <div>
            <div class="experience-tittle title-anchor">Armstrongs Accountancy Limited</div>
            <div class="experience-first-info">2yrs 11mos</div>
            <div class="experience-second-info">Coventry, United Kingdom</div>
          </div>
          <div class="sub-experience">
            <div class="experience-tittle title-anchor">Senior Accountant</div>
            <div class="experience-first-info">Full-time</div>
            <div class="experience-second-info">
              Jul 2021 - Sep 2022 · 1 yr 3 mos
            </div>
            <div class="experience-skills">
              <strong>Skills:</strong> Personal tax · Income Tax · UK
              Corporation Tax · Internal Communications · External
              Communications · External Audits · Capital Gains Tax · Bookkeeping
              · Self Assessment · Accounts Production
            </div>
          </div>
          <div class="sub-experience">
            <div class="experience-tittle title-anchor">Semi Senior Accountant</div>
            <div class="experience-first-info">
              Nov 2019 - Jul 2021 . 1yr 9 mos
            </div>
            <div class="experience-skills">
              <strong>Skills:</strong> Bookkeeping · Self Assessment
            </div>
          </div>
        </div>
      </div>

      <div class="experience-divisor"></div>

      <div class="experience">
        <div>
          <img
            class="company-logo"
            src="https://media.licdn.com/dms/image/C4E0BAQHaT0cdmSpKFg/company-logo_100_100/0/1673379477461/onthegoaccountants_logo?e=1710374400&v=beta&t=-0VSgi0dEWdCcHNdvX8rmput0A-Mn8Au4eR59YDkSrQ"
          />
        </div>
        <div>
          <div>
            <div class="experience-tittle">Accounts Assistant</div>
            <div class="experience-first-info">
              CHARTAC PRACTICE LIMITED · Full-time
            </div>
            <div class="experience-second-info">
              Nov 2016 - Nov 2019 · 3 yrs 1 mo
            </div>
            <div class="experience-second-info">
              Birmingham, England, United Kingdom
            </div>
            <div class="experience-skills">
              <strong>Skills:</strong> VAT Returns · VAT Registration · Payroll
              Services · Property Tax · Bookkeeping · Accounts ProductionSkills
            </div>
          </div>
        </div>
      </div>
    </div>
  </Card>
</template>

<script setup>
import Card from "~/components/Card.vue";
</script>

<style scoped>
.title-anchor:hover{
  color: #0a66c2;
  text-decoration: underline;
  cursor: pointer;
}

.section-tittle {
  font-size: 1.3rem;
  font-weight: 600;
  padding: 1rem 0;
}

.experience-container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;

  .experience-divisor {
    border-top: 1px solid #ccc;
    margin: 0.5rem 0;
  }
}

.experience {
  display: flex;
  gap: 0.5rem;

  .experience-tittle {
    font-size: 1rem;
    font-weight: bold;
  }

  .experience-first-info {
    font-size: 0.9rem;
    color: #2e2e2e;
  }

  .experience-second-info {
    font-size: 0.9rem;
    color: #666;
  }

  .experience-skills {
    font-size: 0.9rem;
    padding-top: 12px;
  }
}

.sub-experience {
  padding: 1rem 0;
}
</style>
