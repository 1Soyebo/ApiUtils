# ApiUtils
A swift class with static methods that utilise Alamofire to call backend apis and handle the response on success and failure through closures 

/*
private func presentCameraView(){
    let vc = UIImagePickerController()
    vc.sourceType = .camera
    vc.allowsEditing = true
    vc.delegate = self
    SaveState.savedState = SaveState(firstname: firstname ?? "", lastname: lastname ?? "", phoneNumber: phoneNumber ?? "", emailAddress: emailAddress ?? "", gender: gender ?? "", promoCode: promoCode ?? "")
    present(vc, animated: true)
}
*/

/*
extension CreateAccountTelemedicineViewController: UINavigationControllerDelegate, UIImagePickerControllerDelegate{
    func imagePickerController(_ picker: UIImagePickerController, didFinishPickingMediaWithInfo info: [UIImagePickerController.InfoKey : Any]) {
        
        picker.dismiss(animated: true)
        guard let image = info[.editedImage] as? UIImage else {
            print("No image found")
            return
        }
        
        let numberOfFacesDetected = detectFaces(imageSelected: image)
        if numberOfFacesDetected < 1{
            presentOkAlert("Error", "No faces detected", handler: nil)
            return
        }else if numberOfFacesDetected > 1 {
            presentOkAlert("Error", "More than one image in photo", handler: nil)
            return
        }
        
        DispatchQueue.main.async {[weak self] in
            self?.imgProfilePhoto.image = image
        }
        
        base64String = image.jpegData(compressionQuality: 0.1)!.base64EncodedString()
        // print out the image size as a test
    }
    
    func detectFaces(imageSelected: UIImage) -> Int {
        let faceImage = CIImage(image: imageSelected)
        let faceDetector = CIDetector(ofType: CIDetectorTypeFace, context: nil, options: [CIDetectorAccuracy: CIDetectorAccuracyHigh])
        let faces = faceDetector?.features(in: faceImage!) as! [CIFaceFeature]
        return faces.count
    }
    
}
*/
