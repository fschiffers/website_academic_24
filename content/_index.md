---
# Leave the homepage title empty to use the site title
title:
date: 2024-04-14
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: 
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ['20px', '0', '20px', '0']
  - block: markdown
    content:
      title: Selected Publications
      text:
        <table>
          <tr>
            <td>
              <img src="images/thumbnails/multisource.png" alt="MultiSource Holography" width="400">
            </td>
            <td>
              <span style="font-size:2em;">MultiSource Holography</span>
              <br>
               Grace Kuo, <b>Florian Schiffers</b>, Douglas Lanman, Oliver Cossairt and Nathan Matsuda
              <i>Interstellar Journal of Advanced Research 2024</i>
              <br>
              <a href="https://arxiv.org/abs/2309.10816">arXiv</a> | <a href="https://grace-kuo.com/resources/multisource_supplement.pdf">Supplement</a>
              <br>
              We propose an architecture for speckle reduction in holographic displays that uses an array of mutually incoherent sources and two sequential spatial light modulators. Multisource holography can suppress speckle in a single frame without sacrificing resolution.
            </td>
          </tr>
          <tr>
            <td>
              <img src="images/thumbnails/stochastic_light_field_holography.png" alt="Quantum Flux Capacitors" width="400">
            </td>
            <td>
              <span style="font-size:2em;">Stochastic Lightfield Holography</span>
              <br>
               <b>Florian Schiffers</b>, Praneeth Chakravarthula, N. Matsuda, G. Kuo, E. Tseng, D. Lanman, F. Heide, Oliver Cossairt
              <i>ICCP 2023</i>
              <br>
              <a href="https://light.princeton.edu/wp-content/uploads/2023/08/stochastic_light_field_holography_supp.pdf">arXiv</a> | <a href="https://website-name.com">Supplement</a>
              <br>
              Our novel hologram generation algorithm enhances the realism of near-eye displays by matching the projection operators of incoherent (Light Field) and coherent (Wigner Function) light transport. By supervising hologram computation with on-the-fly synthesized photographs using Light Field refocusing, our method significantly improves image quality and viewing experience across diverse pupil states.
            </td>
          </tr>
          <tr>
            <td>
              <img src="images/thumbnails/ct.png" alt="Neutrino Particle Simulation" width="400">
            </td>
            <td>
              <span style="font-size:1.5em;">2-Step Sparse-View CT Reconstruction with a Domain-Specific Perceptual Network</span>
              <br>
              <b>Florian Schiffers*</b>, Haoyu Wei*, Tobias Wuerfl, Daming Shen, Daniel Kim, Aggelos Katsaggelos, Oliver Cossairt
              <br>
              <a href="https://arxiv.org/abs/2309.10816">arXiv</a> | <a href="https://website-name.com">Supplement</a>
              <br>
              Our novel framework for sparse-view computed tomography overcomes the challenges of angular undersampling by using a super-resolution network and a refinement network, resulting in high-quality reconstructions with significantly reduced streak artifacts. Our method enhances domain-specific information and demonstrates a 4 dB improvement over current solutions.
            </td>
          </tr>
          <tr>
            <td>
              <img src="images/thumbnails/selvie.png" alt="Selfvi Self-supervised light-field video reconstruction from stereo video" width="400">
            </td>
            <td>
              <span style="font-size:1.5em;">Selfvi Self-supervised light-field video reconstruction from stereo video</span>
              <br>
              Prasan Shedligeri, <b>Florian Schiffers</b>, Sushobhan Ghosh, Oliver Cossairt, Kaushik Mitra
              <i>ICCV 2021</i>
              <br>
              <a href="https://openaccess.thecvf.com/content/ICCV2021/papers/Shedligeri_SeLFVi_Self-Supervised_Light-Field_Video_Reconstruction_From_Stereo_Video_ICCV_2021_paper.pdf">paper</a> | <a href="https://openaccess.thecvf.com/content/ICCV2021/supplemental/Shedligeri_SeLFVi_Self-Supervised_Light-Field_ICCV_2021_supplemental.zip">Supplement</a>
              <br>
              Light-field imaging is attractive for mobile devices due to its intuitive post-capture processing, though acquiring high-quality LF data is challenging with space constraints. We propose a self-supervised algorithm for reconstructing high-fidelity LF videos from stereo videos, leveraging geometric and temporal information and enables applications like post-capture focus control.
            </td>
          </tr>
        </table>
    design:
      columns: '1'
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ['25px', '0', '10px', '0']
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: 
      #Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      email: florianschiffers+fromwebsite@gmail.com
      # phone: +1 872 235 6608
      appointment_url: 'https://florianschiffers.youcanbook.me/'
      # address:
      #   street: 450 Serra Mall
      #   city: Stanford
      #   region: CA
      #   postcode: '94305'
      #   country: United States
      #   country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      # contact_links:
      #   - icon: twitter
      #     icon_pack: fab
      #     name: DM Me
      #     link: 'https://twitter.com/Twitter'
        # - icon: skype
        #   icon_pack: fab
        #   name: Skype Me
        #   link: 'skype:echo123?call'
        # - icon: video
        #   icon_pack: fas
        #   name: Zoom Me
        #   link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
    design:
      columns: '2'
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ['20px', '0', '20px', '0']

---
