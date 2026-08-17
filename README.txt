KarNet Firebase + Cloudinary — Blog/Resources Sync

GitHub Pages structure:
- index.html = public customer website
- admin/index.html = owner login + dashboard

Connected:
- Firebase Authentication
- Firestore shared content under karnetSite/{document}
- Cloudinary cloud: xay1rk6z
- Unsigned upload preset: karnet_unsigned

Admin → Public sync:
- Products
- Solutions
- FAQs
- Testimonials
- Blog / Resources
- Website content/settings

Blog / Resources:
- Add/Edit/Delete/Publish/Unpublish in Admin
- Published posts automatically appear under Resources on customer site
- Featured image supports Cloudinary drag & drop or Browse
- Draft/Scheduled posts stay hidden publicly

Design/layout preserved; changes are functionality additions to the existing design.


ENQUIRY/DEMO FIX:
- Public submissions can create even if a Firebase owner session exists in the same browser.
- Customer success is only shown after Firestore confirms the write.
- Admin listens live to enquiries, demo requests and broadband requests.

PROFILE SYNC FIX:
- Admin Profile Name + Email now save to Firestore.
- Profile Name is mirrored to the public Contact company name.
- Profile Email is mirrored to the public Contact email.
- Contact Information address/phone remain controlled by Settings > Contact Information.

MAP SYNC FIX:
- Contact map now renders from settings.contact.map.
- Google Maps share links open via an overlay button.
- Actual Maps embed URLs are embedded directly.
- If a short share link is supplied, map embed is generated from the saved address.


GLOW CARD UPDATE:
- Pointer-following GlowCard effect translated from supplied React component into plain CSS/JS.
- Applied to customer-facing cards, map block, contact form block, resource/blog cards, product cards, modal blocks, and major bordered content blocks.
- Existing layout/design structure preserved.
- Real Google map sync remains functional.

LATEST UI UPDATE:
- Testimonials use continuous marquee cards, pause on hover, still driven by Firestore admin Testimonials.
- Hero uses a scroll-reactive perspective/scale animation adapted from the provided ContainerScroll React example.
- Contact location uses an interactive Cobe globe visual centered on Tumakuru; owner-managed Google Maps URL remains the Open Maps link.
- Existing Firebase, Cloudinary, enquiries, demo requests, products, FAQs, blog/resources and admin layout retained.


Latest UI update: Home hero replaced with interactive WebGL shader hero adapted from supplied React component. Existing Firebase content sync and CTA actions preserved.

SITE-WIDE SHADER THEME UPDATE
- Public website palette matched to WebGL shader hero.
- Light sections converted to deep black/navy surfaces with cyan/teal accents.
- Existing layouts, Firebase sync, Cloudinary, admin panel, FAQ, testimonials and globe are preserved.

- New products added from Owner Login now render with the same full KANBAN360-style product layout (overview card + description + feature bullets + CTAs).


FINAL FIX:
- Restored interactive WebGL shader hero UI.
- Add/Edit Product now has Feature 1-4 fields.
- Up to four entered features render as teal tick bullets in the public KANBAN360-style product layout.


LATEST FIXES:
- Removed public karnet.co.in contact line
- Dynamic products: content first on mobile; alternating left/right on desktop
- Responsive product cards/buttons on all screen sizes
- New KarNet Broadband logo in public header/footer and admin branding
- Admin dashboard renders charts/products/solutions immediately before Firebase sync

Submission success page:
- thanks.html = shown after Contact Message, Enquiry, Demo Request, or Broadband Request is saved successfully.
- Submissions are stored in karnet_enquiries, karnet_demoRequests, and karnet_broadbandRequests for Admin.
