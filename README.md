<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/css/bootstrap.min.css" rel="stylesheet">
    <title>Examroom.AI Helpdesk</title>
</head>
<body>
    <div class="container py-5">
        <div class="row">
            <div class="col-lg-5 col-md-8 mx-auto shadow border bg-white p-4 rounded">
                <img src="https://examroom.ai/client/assets/images/ex_ai_logo.png" alt="logo" width="90%" />
                <h2 class="text-center fw-bold mb-3">Incident Report Form</h2>
                <form name="google-sheet">
                    <div id="form_alerts"></div>
                    <div class="form-group mb-3">
                        <label for="Date & Time" class="form-label">Date & Time</label>
                        <input type="datetime-local" id="Date & Time" name="Date & Time" class="form-control" required>
                    </div>
                    <div class="form-group mb-3">
                        <label for="name" class="form-label">Candidate Name</label>
                        <input type="text" id="name" name="Candidate name" class="form-control" placeholder="Enter Candidate name" required>
                    </div>
                    <div class="form-group mb-3">
                        <label for="email" class="form-label">Candidate Email</label>
                        <input type="email" id="email" name="Candidate email" class="form-control" placeholder="Enter email address" required>
                    </div>
                    <div class="form-group mb-3">
                        <label for="Contact number" class="form-label">Contact Number</label>
                        <input type="Contact Number" id="Contact Number" name="Contact Number" class="form-control" placeholder="Enter Candidate contact number" required>
                    </div>
                    <div class="form-group mb-3">
                        <label for="Exam Name" class="form-label">Exam Name</label>
                        <input type="Exam Name" id="email" name="Exam Name" class="form-control" placeholder="Enter Exam Name" required>
                    </div>
                    <div class="form-group mb-3">
                        <label for="Client Name" class="form-label">Client Name</label>
                        <select id="Client Name" name="Client Name" class="form-control"required>
                            <option value="Client Name">---Select client Name---</option>
                            <option value="American Academy of Ophthalmology/AAO">American Academy of Ophthalmology/AAO	</option>
                            <option value="Credentia/Pennsylvania">Credentia/Pennsylvania</option>
                            <option value="Credentia/Alabama">Credentia/Alabama</option>
                            <option value="Credentia/Colorado">Credentia/Colorado</option>
                            <option value="Credentia/Maryland">Credentia/Maryland</option>
                            <option value="Credentia/Mississippi">Credentia/Mississippi</option>
                            <option value="Credentia/North Carolina(Nurse Aide)">Credentia/North Carolina(Nurse Aide)</option>
                            <option value="Credentia/North Carolina(Med Aide)">Credentia/North Carolina(Med Aide)</option>
                            <option value="Credentia/Rhode Island">Credentia/Rhode Island</option>
                            <option value="Credentia/South Carolina">Credentia/South Carolina</option>
                            <option value="Credentia/Virginia">Credentia/Virginia</option>
                            <option value="Credentia/Washington">Credentia/Washington</option>
                            <option value="Credentia/Georgia">Credentia/Georgia</option>
                            <option value="NOCTI Student">NOCTI Student</option>
                            <option value="NOCTI Business">NOCTI Business</option>
                            <option value="Texas Land Title Prov">Texas Land Title Prov</option>
                            <option value="Event Leadership Institute / ELI">Event Leadership Institute / ELI</option>
                            <option value="National Council of State Boards of Nursing / NCSBN_IRP">National Council of State Boards of Nursing / NCSBN_IRP</option>
                            <option value="National Council of State Boards of Nursing / NCSBN">National Council of State Boards of Nursing / NCSBN</option>
                            <option value="Performance Programs/Terry">Performance Programs/Terry</option>
                            <option value="PMI (ER/Prov)">PMI (ER/Prov)</option>
                            <option value="ABMCN/CMCN/Jakie">ABMCN/CMCN/Jakie</option>
                            <option value="Debbie/CICM">Debbie/CICM</option>
                            <option value="Biofeedback Certification International Alliance(BCIA)">Biofeedback Certification International Alliance(BCIA)</option>
                            <option value="ETAI">ETAI</option>
                            <option value="Institute of business Forecasting / IBF">Institute of business Forecasting / IBF</option>
                            <option value="Dexter/RPA/SmartAutomation">Dexter/RPA/SmartAutomation</option>
                            <option value="NWCU">NWCU</option>
                            <option value="American Board of Cardiovascular Medicine (ABCM)">American Board of Cardiovascular Medicine (ABCM)</option>
                            <option value="Language Testing International (LTI)">Language Testing International (LTI)</option>
                            <option value="Mirakl University">Mirakl University</option>
                            <option value="IAEI">IAEI</option>
                            <option value="ICHCC">ICHCC</option>
                            <option value="PAHCOM">PAHCOM</option>
                            <option value="National Insulation Association (NIA)">National Insulation Association (NIA)</option>
                            <option value="FAA">FAA</option>
                            <option value="SpaceTech">SpaceTech</option>
                            <option value="Certified Exit Planning Institue / CEPA">Certified Exit Planning Institue / CEPA</option>
                            <option value="ABYC / American Boat and Yachtn Council">ABYC / American Boat and Yachtn Council</option>
                            <option value="American Translators Association/ ATA">American Translators Association/ ATA</option>
                            <option value="National Center for Competency Testing / NCCT">National Center for Competency Testing / NCCT</option>
                            <option value="Spearhead Training">Spearhead Training</option>
                            <option value="AAEES">AAEES</option>
                            <option value="ISCET">ISCET</option>
                            <option value="State Food Safety / SFS">State Food Safety / SFS</option>
                            <option value="NOCTI Exams || Cleveland State ">NOCTI Exams || Cleveland State </option>
                            <option value="Freshman Institute">Freshman Institute</option>
                            <option value="Association for Health Care Documentation Integrity">Association for Health Care Documentation Integrity</option>
                            <option value="Fresh Works">Fresh Works</option>
                            <option value="Roundstone Consulting">Roundstone Consulting</option>
                            <option value="SouthWest Mississippi Community College">SouthWest Mississippi Community College</option>
                        </select>    
                    </div>
                    <div class="form-group mb-3">
                        <label for="Type Issue" class="form-label">Type Issue</label>
                        <textarea id="Type Issue" name="Type Issue faced by candidate" class="form-control" placeholder="Enter The Issue" rows="5" required></textarea>
                    </div>
                    <div class="form-group mb-3">
                        <label for="Resolution" class="form-label">Resolution</label>
                        <textarea id="Resolution" name="Resolution Provided" class="form-control" placeholder="Enter Resolution provided" rows="5" required></textarea>
                    </div>
                    <div class="form-group mb-3">
                        <label for="Status of exam" class="form-label">Status of exam</label>
                        <textarea id="Status of exam" name="Status of exam" class="form-control" placeholder="Status of Exam" rows="5" required></textarea>
                    </div>
                    <div class="form-group mb-3">
                        <label for="Agent Name" class="form-label">Issue reported by</label>
                        <input type="Agent Name" id="Agent Name" name="Agent Name" class="form-control" placeholder="Please enter Agent Name" required>
                    </div>
                    <div>
                        <button class="btn btn-primary me-2" type="submit">Send Incident Report!</button>
                        <button class="btn btn-danger" type="reset">Reset the form!</button>
                    </div>
                </form>
            </div>
        </div>
    </div>

    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        const scriptURL = 'https://script.google.com/macros/s/AKfycbyJS341vQh5dfMTa1IxkgCcK0jJJi5sCBCIiRIFych3UfARLWN1edCpiJ1FsTtMmwk/exec'
        const form = document.forms['google-sheet']
        
        form.addEventListener('submit', e => {
            e.preventDefault()
            fetch(scriptURL, { method: 'POST', body: new FormData(form)})
            .then(response => $("#form_alerts").html("<div class='alert alert-success'>Incident Report sent successfully.</div>"))
            .catch(error => $("#form_alerts").html("<div class='alert alert-danger'>Incident Report not sent.</div>"))
        })
    </script>
</body>
</html>
</body>
</html>
