Vagrant.configure("2") do |config|
  config.vm.box = "google/gce"

  config.vm.provider :google do |google, override|
    google.google_project_id = "alien-bricolage-212412"
    google.google_client_email = "devopskishore9@gmail.com"
    google.google_json_key_location = "/Users/ninja/Downloads/gcpkey.json"
    #google.name = "my-test-instance"
    google.name = "my-test-instance"
    
    #google.image_family = 'ubuntu-1604-lts'
    google.image_family = 'centos-7'
    
    override.ssh.username = "ninja"
    override.ssh.private_key_path = "~/.ssh/id_rsa"
    #override.ssh.private_key_path = "~/.ssh/google_compute_engine"
  end

end
