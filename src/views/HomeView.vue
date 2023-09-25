<template>
  <div>
    <v-container id="resumeCard" ref="resumeCard" class="px-0">
      <v-row>
        <v-col cols="12" class="mx-2 pa-0">
          <div class="text-left text-wrap font-weight-bold primary--text Heading">DHANUNJAYA REDDY</div>
        </v-col>
        <v-col cols="12" class="pa-0 mx-2">
          <div class="text-left primary--text Heading3">AWS Developer | NodeJS Developer</div>
        </v-col>
        <v-col cols="12" class="pa-0 mx-2">
          <p class="text-justify primary--text about">
            Experienced Microservices AWS Developer with 4+ years of expertise designing, developing, and building efficient microservices
            architecturesusing Node.js. Proficient in optimizing performance, integrating AWS services and leveraging industry best practices to
            create robust andscalable cloud-native applications. Adept at collaborating with cross-functional teams to deliver high-quality solutions.
          </p>
        </v-col>
        <v-row>
          <v-col cols="3" class="primary--text font-weight-bold"><v-icon color="primary">mdi-phone</v-icon> +91 9036383353</v-col>
          <v-col cols="4" class="primary--text font-weight-bold"><v-icon color="primary">mdi-email</v-icon><a>dhanunjay18184@gmail.com</a> </v-col>
          <v-col cols="3" class="primary--text font-weight-bold"><v-icon color="primary">mdi-map-marker</v-icon>Bangalore,India</v-col>
          <v-col cols="2" class="primary--text font-weight-bold"
            ><a style="text-decoration: none; cursor: pointer" href="https://www.linkedin.com/in/dhanunjaya-reddy-3a3413221" target="_blank"
              ><v-icon color="primary">mdi-linkedin</v-icon>dhanunujaya</a
            ></v-col
          >
        </v-row>
        <v-col cols="12" class="mt-2">
          <v-row class="">
            <v-col class="skills-card px-4" cols="4">
              <div class="text-left Heading3">Technical Skills</div>
              <hr />
              <ul class="pa-2 text-left" id="" v-for="(techs, i) in TechnicalSkills" :key="i">
                <div class="font-weight-bold">
                  {{ techs.heading }}
                </div>
                <li class="ml-4" v-for="(skill, i) in techs.skills" :key="i">{{ skill }}</li>
              </ul>
            </v-col>
            <v-col cols="8" class="pt-0 pr-0">
              <div class="Heading2 font-weight-bold text-left pa-0">Experience</div>
              <hr width="50%" />
              <v-timeline align-top dense class="">
                <v-timeline-item color="primary" small class="pl-0 ml-o">
                  <div class="Heading4 primary--text text-left">Mobil80 Solutions and Services Pvt Ltd.</div>
                  <small class="font-weight-bold py-2 primary--text text-left experience-sub"
                    >2020 August - Present Day | 3+ Years | Software Developer</small
                  >
                  <small class="font-weight-bold py-2 primary--text experience-sub">Role</small>
                  <p class="experience-content text-justify primary--text">
                    Leading a team of backend developers, driving microservices architecture, anddelivering innovative service-based projects and
                    blockchain solutions. Proactivelyexploring emerging technologies to enhance products and contributing to in-houseinitiatives.
                  </p>
                  <div class="Heading5 primary--text text-left">Projects</div>
                  <div class="about font-weight-bold primary--text py-2 text-left">1. Vozcare - CRM And Inbuilt Dialer. | Client Location - UAE</div>
                  <div class="pr-0">
                    <ul>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Robust Backend Architecture: </span
                        ><span class="experience-content text-justify primary--text"
                          >Orchestrated backend with AWS microservices andEC2 hosting. Leveraged DynamoDB for efficient data management</span
                        >
                      </li>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Seamless Integration, Data Security: </span
                        ><span class="experience-content text-justify primary--text"
                          >Integrated lead management, email, SMS,voice services via Asterisk and SNS. Employed Cognito, AppSync for real-timedata,
                          Amazon S3 for secure call recordings. Segregated lead data on client'saccount for privacy.</span
                        >
                      </li>
                    </ul>
                  </div>
                  <div class="about font-weight-bold primary--text text-left pt-3 pb-2">
                    2. XcelAudit - Comprehensive Auditing System | Client Location - India
                  </div>
                  <div class="pr-0">
                    <ul>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Innovative Engineered Solution: </span
                        ><span class="experience-content text-justify primary--text"
                          >"XcelAudit" utilized AWS DynamoDB andLambda for dynamic rule processing, ensuring precise compliance.</span
                        >
                      </li>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Enhanced Date Management: </span
                        ><span class="experience-content text-justify primary--text"
                          >AWS EventBridge ensured accurate date tracking,strengthening auditing accuracy..</span
                        >
                      </li>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Integrated Insights & Security: </span
                        ><span class="experience-content text-justify primary--text"
                          >Seamless AWS service integration, includingCognito and AppSync, boosted security and workflows. Dashboards, PDFreports, and
                          action logs facilitated comprehensive auditing.</span
                        >
                      </li>
                    </ul>
                  </div>
                  <div class="about font-weight-bold primary--text pt-3 pb-2 text-left">
                    3. Cabinet - Advance Cloud Storage System | Client Location - USA
                  </div>
                  <div class="pr-0">
                    <ul>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Tailored Workflows: </span
                        ><span class="experience-content text-justify primary--text"
                          >"Cabinet" introduces personalized workflows fordocuments and quizzes, optimizing user processes. (AWS technologies:
                          Athena,DynamoDB).</span
                        >
                      </li>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Selective Access Control: </span
                        ><span class="experience-content text-justify primary--text"
                          >Leveraging Athena, "Cabinet" empowers granulardocument sharing, ensuring data security and controlled access.</span
                        >
                      </li>
                      <li class="pr-0 text-justify">
                        <span class="about font-weight-bold primary--text">Real-time Notifications: </span
                        ><span class="experience-content text-justify primary--text"
                          >Through SES, "Cabinet" triggers targeted email alertsfor document-related events, enhancing user engagement and
                          awareness.</span
                        >
                      </li>
                    </ul>
                  </div>
                </v-timeline-item>
              </v-timeline>
              <div class="Heading2 font-weight-bold text-left pa-0">Education</div>
              <hr width="50%" />
              <div class="Heading5 primary--text text-left ml-3">Presidency University | 2015 - 2019</div>
              <div class="primary--text ml-3 text-left">B-Tech in Computer Science & Engineering</div>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>

    <div>
      <v-btn class="text-capitalize buttonBackground font-weight-bold ma-4" rounded large dark @click="downloadResumeAsPDF"
        >Download My CV Here</v-btn
      >
    </div>
  </div>
</template>
<script>
import jsPDF from "jspdf";
export default {
  name: "MyResume",
  data: () => ({
    TechnicalSkills: [
      {
        heading: "Cloud Technologies",
        skills: [
          "Lambda",
          "SAM CLI",
          "EC2",
          "Cognito",
          "API Gateway",
          "Appsync",
          "Dynamo DB",
          "Aurora Serverless",
          "AWS RDS",
          "AWS S3",
          "AWS SES",
          "AWS SNS",
          "CloudSearch",
          "Cloudwatch",
          "Route53",
          "Cloudfront",
        ],
      },
      {
        heading: "Database & Analytics",
        skills: ["Dynamo DB", "Mongo DB", "MySQL", "PostgreSQL"],
      },
      {
        heading: "Other Technolgies",
        skills: [
          "VerneMQ - MQTT",
          "IOT Core And Arduino",
          "SAM CLI and Github as Pipeline",
          "Arweave Blockchain",
          "Websocket",
          "Asterisk",
          "Tableau",
        ],
      },
    ],
  }),
  methods: {
    downloadResumeAsPDF() {
      const resumeElement = document.getElementById("resumeCard");
      console.log(resumeElement);
      const pdf = new jsPDF();
      const pdfOptions = {
        format: "a4",
        orientation: "portrait",
      };
      this.$nextTick(() => {
        pdf.html(resumeElement, pdfOptions, () => {
          pdf.save("my_resume.pdf");
        });
      });
    },
  },
};
</script>
<style scoped>
.Heading {
  font-size: 50px;
}
.Heading2 {
  font-size: 35px;
}
.Heading3 {
  font-size: 25px;
}
.Heading4 {
  font-size: 20px;
}
.Heading5 {
  font-size: 18px;
}
.about {
  font-size: 14px;
}

.skills-card {
  background: #273447;
  color: white;
}
.experience-sub {
  word-spacing: 8px;
}
.experience-content {
  font-size: 13px;
}
.buttonBackground {
  background: rgb(2, 0, 36);
  background-image: linear-gradient(90deg, rgba(2, 0, 36, 1) 0%, rgba(9, 9, 121, 1) 35%, rgba(0, 212, 255, 1) 100%);
}
</style>
