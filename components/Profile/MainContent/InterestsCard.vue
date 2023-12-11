<template>
  <Card>
    <div class="section-tittle">Interests</div>

    <div class="interests-tabs">
      <div @click="tabChosen = 1">
        <button>Companies</button>
        <div v-if="tabChosen === 1" class="chosen"></div>
      </div>

      <div @click="tabChosen = 2">
        <button>Groups</button>
        <div v-if="tabChosen === 2" class="chosen"></div>
      </div>

      <div @click="tabChosen = 3">
        <button>Newsletters</button>
        <div v-if="tabChosen === 3" class="chosen"></div>
      </div>

      <div @click="tabChosen = 4">
        <button>Schools</button>
        <div v-if="tabChosen === 4" class="chosen"></div>
      </div>
    </div>
    <div>
      <div>
        <div v-if="tabChosen === 1" class="interest-content">
          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/C560BAQGNtpblgQpJoQ/company-logo_100_100/0/1662120928214/deloitte_logo?e=1710374400&v=beta&t=rPyENktVwCS3FPtNjgyJvlNROh9BJfLUquIzZuoxCQw"
              />
            </div>
            <div>
              <div class="interest-tittle">Deloitte</div>
              <div class="interest-second">13,953,943 followers</div>
              <WhiteButton>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 16 16"
                  height="16"
                  width="16"
                >
                  <path
                    d="M0 8a1 1 0 0 0 1 1h5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 0.16666666666666666v5.833333333333333a1 1 0 0 0 2 0v-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 -0.16666666666666666h5.833333333333333a1 1 0 0 0 0 -2h-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 -0.16666666666666666V1a1 1 0 0 0 -2 0v5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 0.16666666666666666H1A1 1 0 0 0 0 8Z"
                    fill="#5e5e5e"
                    stroke-width="0.6666666666666666"
                  ></path>
                </svg>
                <span>Follow</span>
              </WhiteButton>
            </div>
          </div>

          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/D4D0BAQH3qXh7nyImoQ/company-logo_100_100/0/1697100791441/pwc_logo?e=1710374400&v=beta&t=QWC0mX64Vs52Cp7e4orXSeCAXYa_T7INtunrES3fPNo"
              />
            </div>

            <div>
              <div class="interest-tittle">PwC</div>
              <div class="interest-second">5,747,474 followers</div>
              <WhiteButton>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 16 16"
                  height="16"
                  width="16"
                >
                  <path
                    d="M0 8a1 1 0 0 0 1 1h5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 0.16666666666666666v5.833333333333333a1 1 0 0 0 2 0v-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 -0.16666666666666666h5.833333333333333a1 1 0 0 0 0 -2h-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 -0.16666666666666666V1a1 1 0 0 0 -2 0v5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 0.16666666666666666H1A1 1 0 0 0 0 8Z"
                    fill="#5e5e5e"
                    stroke-width="0.6666666666666666"
                  ></path>
                </svg>
                <span>Follow</span>
              </WhiteButton>
            </div>
          </div>
        </div>

        <div v-if="tabChosen === 2" class="interest-content">
          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/C5607AQE66xzWae_7Rg/group-logo_image-shrink_48x48/0/1631008780854?e=1702764000&v=beta&t=rIbkM0QQcu0oAive_44gUpY9B3cn0yNMOdQsPw8KL74"
              />
            </div>

            <div>
              <div class="interest-tittle">
                Lead Generation and Sales Hacks Forum
              </div>
              <div class="interest-second">3,959 members</div>
              <WhiteButton>Join</WhiteButton>
            </div>
          </div>

          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/C5607AQFx6ovD4fHuNg/group-logo_image-shrink_48x48/0/1631417575855?e=1702764000&v=beta&t=Qr7-Vdh6w3thrLW-KWJD_pipvsbQRYgJr7E-nJXMTIM"
              />
            </div>

            <div>
              <div class="interest-tittle">ACCA Global Community</div>
              <div class="interest-second">154,817 members</div>
              <WhiteButton>Join</WhiteButton>
            </div>
          </div>
        </div>

        <div v-if="tabChosen === 3" class="interest-content">
          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/D4E12AQFNKHWn9vW7iw/series-logo_image-shrink_100_100/0/1701114044842?e=1707350400&v=beta&t=Ayhk5aUQqBcE_be0tQIEKVoqsBL2-tYcRa9qdUfuRZ8"
              />
            </div>

            <div>
              <div class="interest-tittle">WSJ Networking Challenge</div>
              <div class="interest-first">
                A five-week course covering the emails you need to send before
                the New Year to boost your career.
              </div>
              <div class="interest-second">Published weekly</div>

              <div class="interest-author-container">
                <img
                  class="interest-image-small"
                  src="https://media.licdn.com/dms/image/C4D0BAQErTDc9V8YLdg/company-logo_100_100/0/1630536546293/the_wall_street_journal_logo?e=1710374400&v=beta&t=ig73gVQRvjAz6AJqPhPBt8Mq5t4vcqCsk-lkfrkjMwI"
                />
                <div class="interest-author-tittle">
                  The Wall Street Journal
                </div>
              </div>

              <WhiteButton>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 16 16"
                  height="16"
                  width="16"
                >
                  <path
                    d="M0 8a1 1 0 0 0 1 1h5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 0.16666666666666666v5.833333333333333a1 1 0 0 0 2 0v-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 -0.16666666666666666h5.833333333333333a1 1 0 0 0 0 -2h-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 -0.16666666666666666V1a1 1 0 0 0 -2 0v5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 0.16666666666666666H1A1 1 0 0 0 0 8Z"
                    fill="#5e5e5e"
                    stroke-width="0.6666666666666666"
                  ></path>
                </svg>
                <span>Follow</span>
              </WhiteButton>
            </div>
          </div>

          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/D5612AQEXsyCHnmNhRw/series-logo_image-shrink_100_100/0/1691019769841?e=1707350400&v=beta&t=n6_V8lMtbJksb4RTUnoozq_MacdZbZu8MIpkI9GZMrE"
              />
            </div>

            <div>
              <div class="interest-tittle">The Retail Roundup</div>
              <div class="interest-first">
                Level up your retail game with Salesforce's industry insights,
                shopping trends, and insider tips.
              </div>
              <div class="interest-second">Published monthly</div>

              <div class="interest-author-container">
                <img
                  class="interest-image-small"
                  src="https://media.licdn.com/dms/image/C560BAQHZ9xYomLW7zg/company-logo_100_100/0/1630658255326/salesforce_logo?e=1710374400&v=beta&t=tBl34cYy2CSB1XsOIK3NBlO-0WUFWQQMu99IZKLWGu8"
                />
                <div class="interest-author-tittle">Salesforce</div>
              </div>

              <WhiteButton>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 16 16"
                  height="16"
                  width="16"
                >
                  <path
                    d="M0 8a1 1 0 0 0 1 1h5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 0.16666666666666666v5.833333333333333a1 1 0 0 0 2 0v-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 -0.16666666666666666h5.833333333333333a1 1 0 0 0 0 -2h-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 -0.16666666666666666V1a1 1 0 0 0 -2 0v5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 0.16666666666666666H1A1 1 0 0 0 0 8Z"
                    fill="#5e5e5e"
                    stroke-width="0.6666666666666666"
                  ></path>
                </svg>
                <span>Follow</span>
              </WhiteButton>
            </div>
          </div>
        </div>

        <div v-if="tabChosen === 4" class="interest-content">
          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/D4E0BAQFhiriQNuluqQ/company-logo_100_100/0/1682266192901/selftaught_logo?e=1710374400&v=beta&t=QHsdd36x_XShWDc8fbXhss--vCUKuGv1nKPEpFDyQKU"
              />
            </div>

            <div>
              <div class="interest-tittle">Self-taught</div>
              <div class="interest-second">7,085 followers</div>
              <WhiteButton>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 16 16"
                  height="16"
                  width="16"
                >
                  <path
                    d="M0 8a1 1 0 0 0 1 1h5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 0.16666666666666666v5.833333333333333a1 1 0 0 0 2 0v-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 -0.16666666666666666h5.833333333333333a1 1 0 0 0 0 -2h-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 -0.16666666666666666V1a1 1 0 0 0 -2 0v5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 0.16666666666666666H1A1 1 0 0 0 0 8Z"
                    fill="#5e5e5e"
                    stroke-width="0.6666666666666666"
                  ></path>
                </svg>
                <span>Follow</span>
              </WhiteButton>
            </div>
          </div>

          <div class="interest">
            <div>
              <img
                class="company-logo"
                src="https://media.licdn.com/dms/image/C560BAQHF0C2pS7GDeg/company-logo_100_100/0/1631366939753?e=1710374400&v=beta&t=W55Ky2ktaa6fPoY9sBKe8by8-5p8T0zZqqOCodYctnM"
              />
            </div>

            <div>
              <div class="interest-tittle">Kaplan Professional</div>
              <div class="interest-second">25,305 followers</div>
              <WhiteButton>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 16 16"
                  height="16"
                  width="16"
                >
                  <path
                    d="M0 8a1 1 0 0 0 1 1h5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 0.16666666666666666v5.833333333333333a1 1 0 0 0 2 0v-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 0.16666666666666666 -0.16666666666666666h5.833333333333333a1 1 0 0 0 0 -2h-5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 -0.16666666666666666V1a1 1 0 0 0 -2 0v5.833333333333333a0.16666666666666666 0.16666666666666666 0 0 1 -0.16666666666666666 0.16666666666666666H1A1 1 0 0 0 0 8Z"
                    fill="#5e5e5e"
                    stroke-width="0.6666666666666666"
                  ></path>
                </svg>
                <span>Follow</span>
              </WhiteButton>
            </div>
          </div>
        </div>
      </div>
    </div>

    <template v-slot:footer>
      <CardFooterButton>Show all {{ names[tabChosen] }}></CardFooterButton>
    </template>
  </Card>
</template>

<script setup>
import Card from "~/components/Card.vue";

const tabChosen = ref(1);

const names = ref({
  1: "Companies",
  2: "Groups",
  3: "Newsletters",
  4: "Schools",
});
</script>

<style scoped>
.section-tittle {
  font-size: 1.25rem;
  font-weight: 600;
}

.interests-tabs {
  display: flex;
  gap: 1rem;

  & button {
    background-color: transparent;
    border: none;
    cursor: pointer;
    font-size: 0.85rem;
    font-weight: 600;
    padding-top: 12px;
    padding-bottom: 16px;
    color: #01754f;

    &:hover {
      color: #004c33;
      background-color: #f3f3f3;
    }
  }

  & .chosen {
    width: 100%;
    height: 2px;
    background-color: #01754f;
  }
}

.interest-content {
  display: flex;
  gap: 1rem;
  padding: 0.8rem 0.5rem;
}

.interest {
  width: 50%;
  display: flex;
  gap: 0.5rem;

  .interest-tittle {
    font-size: 1rem;
    font-weight: 600;
    padding: 2px 0px;

    &:hover {
      cursor: pointer;
      color: #0a66c2;
      text-decoration: underline;
    }
  }

  .interest-first {
    font-size: 0.875rem;
  }

  .interest-second {
    font-size: 0.875rem;
    color: #5e5e5e;
  }
}

.interest-author-container {
  display: flex;
  gap: 0.5rem;
  align-items: center;
  padding: 12px 0px;

  .interest-author-tittle {
    font-size: 0.875rem;

    &:hover {
      cursor: pointer;
      color: #0a66c2;
      text-decoration: underline;
    }
  }

  .interest-image-small {
    width: 24px;
    height: 24px;
  }
}
</style>
