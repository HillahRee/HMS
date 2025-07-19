# HMS
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Mail, Phone, Calendar } from "lucide-react";
import { motion } from "framer-motion";

export default function PluggedMindsTherapy() {
  return (
    <main className="min-h-screen bg-gradient-to-br from-indigo-100 via-white to-purple-100 p-6">
      <motion.h1
        initial={{ opacity: 0, y: -20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.6 }}
        className="text-4xl font-bold text-center text-indigo-700 mb-8"
      >
        Plugged Minds Therapy
      </motion.h1>
      <section className="grid grid-cols-1 md:grid-cols-2 gap-6 items-center">
        <motion.div
          initial={{ opacity: 0, x: -20 }}
          animate={{ opacity: 1, x: 0 }}
          transition={{ duration: 0.6, delay: 0.2 }}
          className="space-y-4"
        >
          <h2 className="text-2xl font-semibold text-indigo-800">
            Mental Wellness for Youth & Young Adults
          </h2>
          <p className="text-gray-700">
            We offer accessible, judgment-free therapy sessions focused on mental
            health challenges like anxiety, stress, trauma, self-esteem, and
            substance use recovery.
          </p>
          <Button>Book a Free Consultation</Button>
        </motion.div>
        <motion.img
          src="https://images.unsplash.com/photo-1607746882042-944635dfe10e"
          alt="Therapy session visual"
          className="rounded-2xl shadow-lg"
          initial={{ opacity: 0, x: 20 }}
          animate={{ opacity: 1, x: 0 }}
          transition={{ duration: 0.6, delay: 0.4 }}
        />
      </section>
      <section className="mt-16 grid gap-8 grid-cols-1 md:grid-cols-3">
        <Card>
          <CardContent className="p-6 space-y-4">
            <h3 className="text-xl font-medium text-indigo-700">Our Approach</h3>
            <p className="text-gray-700">
              We combine CBT, trauma-informed care, and creative therapies to
              empower young minds.
            </p>
          </CardContent>
        </Card>
        <Card>
          <CardContent className="p-6 space-y-4">
            <h3 className="text-xl font-medium text-indigo-700">Confidential Support</h3>
            <p className="text-gray-700">
              All sessions are private and client-centered, ensuring a safe space
              for expression and growth.
            </p>
          </CardContent>
        </Card>
        <Card>
          <CardContent className="p-6 space-y-4">
            <h3 className="text-xl font-medium text-indigo-700">Book a Session</h3>
            <div className="space-y-2">
              <div className="flex items-center gap-2 text-gray-700">
                <Calendar className="w-5 h-5" /> Mon - Fri, 9am - 5pm
              </div>
              <div className="flex items-center gap-2 text-gray-700">
                <Phone className="w-5 h-5" /> +254 712 345678
              </div>
              <div className="flex items-center gap-2 text-gray-700">
                <Mail className="w-5 h-5" /> hello@pluggedmindstherapy.com
              </div>
            </div>
          </CardContent>
        </Card>
      </section>
      <footer className="mt-20 text-center text-sm text-gray-500">
        &copy; 2025 Plugged Minds Therapy. All rights reserved.
      </footer>
    </main>
  );
}
